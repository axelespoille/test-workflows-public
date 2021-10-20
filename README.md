{
  "type": "flopack",
  "version": "1.2.0",
  "created": "2021-10-20T18:13:42.368Z",
  "flags": {
    "auto-transform": true,
    "looseBooleans": true,
    "looseStrings": true,
    "looseNulls": true
  },
  "data": {
    "flos": {
      "832df825-ce20-44d1-8adf-ea05de362154": {
        "id": "832df825-ce20-44d1-8adf-ea05de362154",
        "name": "Exported Notification Flow",
        "description": "",
        "data": {
          "id": null,
          "uuid": "832df825-ce20-44d1-8adf-ea05de362154",
          "display": {
            "preview": [
              {
                "module": "string",
                "name": "compose",
                "kernel": true
              },
              {
                "module": "control",
                "name": "comment",
                "kernel": true
              },
              {
                "module": "slack",
                "name": "sendMessageToChannel2",
                "kernel": false
              },
              {
                "module": "control",
                "name": "callable",
                "kernel": true
              }
            ],
            "isCallable": true
          },
          "tree": {
            "id": 1,
            "name": "all"
          },
          "methods": [
            {
              "joins": {},
              "address": "root:kernel:string:0.0.1:compose",
              "parents": {
                "version": {
                  "address": "root:kernel:string:0.0.1",
                  "key": "0.0.1",
                  "data": {
                    "name": "0.0.1"
                  }
                },
                "channel": {
                  "address": "root:kernel:string",
                  "key": "string",
                  "data": {
                    "name": "string"
                  }
                }
              },
              "uuid": "Ys-ri8GzO",
              "branches": {},
              "node": {
                "key": "compose",
                "data": {
                  "name": "Compose"
                },
                "model": {
                  "type": "method",
                  "_v": 2,
                  "key": "compose",
                  "executable": false,
                  "displayed": true,
                  "async": false,
                  "cooperative": false,
                  "mirrored": false,
                  "inlined": false,
                  "dependencies": [],
                  "timeout": 90000,
                  "idempotent": false,
                  "monitor": false,
                  "webhook": false,
                  "webhookList": false,
                  "webhookConditions": false,
                  "mobile": false,
                  "hooks": {},
                  "policy": {
                    "error": {
                      "type": "finish"
                    }
                  },
                  "metadata": {
                    "id": null,
                    "name": "Compose",
                    "description": "Enter free form text and optionally drag fields into your text like a mail merge."
                  },
                  "meta": {},
                  "config": null,
                  "partnerChannelKeys": null,
                  "inputs": {
                    "extensible": true,
                    "rules": {
                      "*": {
                        "types": [
                          "string"
                        ],
                        "collection": false
                      }
                    },
                    "data": {
                      "TuQ4iVBwk-": {
                        "id": "TuQ4iVBwk-",
                        "group": null,
                        "key": "_text_",
                        "value": {
                          "type": "string",
                          "collection": false,
                          "data": "Flows exported and PR created on https://github.com/asappinc/test-its-okta-workflows. Please review.",
                          "available": [],
                          "error": false
                        },
                        "required": true,
                        "ref": false,
                        "metadata": {
                          "index": 0
                        },
                        "flags": "d"
                      }
                    }
                  },
                  "outputs": {
                    "extensible": false,
                    "data": {
                      "68xmqrJRVe": {
                        "id": "68xmqrJRVe",
                        "group": null,
                        "key": "output",
                        "value": {
                          "type": "string",
                          "collection": false,
                          "data": ""
                        },
                        "ref": false,
                        "metadata": {
                          "index": 0
                        },
                        "_used": true
                      }
                    }
                  },
                  "runtime": {}
                }
              },
              "pins": {
                "68xmqrJRVe": {
                  "4GEkrYQKY": [
                    {
                      "input": "KzlQKseU9",
                      "transform": null
                    }
                  ]
                }
              }
            },
            {
              "joins": {},
              "address": "root:kernel:control:0.0.1:comment",
              "parents": {
                "version": {
                  "address": "root:kernel:control:0.0.1",
                  "key": "0.0.1",
                  "data": {
                    "name": "0.0.1"
                  }
                },
                "channel": {
                  "address": "root:kernel:control",
                  "key": "control",
                  "data": {
                    "name": "control"
                  }
                }
              },
              "uuid": "Euo2yu8PV",
              "branches": {},
              "node": {
                "key": "comment",
                "data": {
                  "name": "Comment"
                },
                "model": {
                  "type": "method",
                  "_v": 2,
                  "key": "comment",
                  "executable": false,
                  "displayed": true,
                  "async": false,
                  "cooperative": false,
                  "mirrored": false,
                  "inlined": false,
                  "dependencies": [],
                  "timeout": 90000,
                  "idempotent": false,
                  "monitor": false,
                  "webhook": false,
                  "webhookList": false,
                  "webhookConditions": false,
                  "mobile": false,
                  "hooks": {},
                  "policy": {
                    "error": {
                      "type": "finish"
                    }
                  },
                  "metadata": {
                    "id": null,
                    "name": "Comment",
                    "description": "Leave a comment."
                  },
                  "meta": {},
                  "config": null,
                  "partnerChannelKeys": null,
                  "inputs": {
                    "extensible": false,
                    "data": {}
                  },
                  "outputs": {
                    "extensible": false,
                    "data": {}
                  },
                  "runtime": {},
                  "display": {},
                  "comments": {
                    "title": "Add a Note",
                    "markdown": "Runs and notifies on Wednesdays and Saturdays at 1am EST."
                  }
                }
              },
              "pins": {}
            },
            {
              "joins": {},
              "address": "root:channels:http:slack:1.6.211:sendMessageToChannel2",
              "parents": {
                "version": {
                  "address": "root:channels:http:slack:1.6.211",
                  "key": "1.6.211",
                  "data": {
                    "name": "1.6.211",
                    "id": 442
                  }
                },
                "channel": {
                  "address": "root:channels:http:slack",
                  "key": "slack",
                  "data": {
                    "name": "slack",
                    "id": 24
                  }
                }
              },
              "uuid": "4GEkrYQKY",
              "branches": {},
              "node": {
                "key": "sendMessageToChannel2",
                "data": {
                  "name": "Send Message to Channel"
                },
                "model": {
                  "type": "method",
                  "_v": 2,
                  "key": "sendMessageToChannel2",
                  "executable": true,
                  "displayed": true,
                  "async": true,
                  "cooperative": false,
                  "mirrored": false,
                  "compat": false,
                  "inlined": false,
                  "dependencies": [],
                  "timeout": 30000,
                  "idempotent": false,
                  "monitor": false,
                  "webhook": false,
                  "webhookList": false,
                  "webhookConditions": false,
                  "mobile": false,
                  "hooks": {},
                  "policy": {
                    "error": {
                      "type": "finish"
                    }
                  },
                  "metadata": {
                    "id": 22780,
                    "name": "Send Message to Channel",
                    "description": null
                  },
                  "meta": {
                    "3b90b67b-6ca2-4fce-8d93-23167ecab8e0": {
                      "id": "rrS1CpdwrBu",
                      "address": {
                        "key": null,
                        "group": null,
                        "groupIndex": 0,
                        "defaultValue": {
                          "method": "makeChannelOrNameInput"
                        },
                        "namespace": "input"
                      }
                    },
                    "fbc05ee9-0db5-465e-9b90-78b6f31374c0": {
                      "id": "yeeHI1LirE1",
                      "address": {
                        "key": null,
                        "group": null,
                        "groupIndex": 1,
                        "defaultValue": {
                          "method": "sendMessageInputs"
                        },
                        "namespace": "input"
                      }
                    },
                    "ab700001-8882-44d1-a788-70d9142887ec": {
                      "id": "h7lbnZkJrmu",
                      "address": {
                        "key": null,
                        "group": null,
                        "groupIndex": 2,
                        "defaultValue": {
                          "method": "slackbotNameInput"
                        },
                        "namespace": "input"
                      }
                    }
                  },
                  "config": "e62cbc79-d44e-4a95-b9e1-e97f19fe6aad",
                  "partnerChannelKeys": 208,
                  "inputs": {
                    "extensible": false,
                    "rules": {},
                    "groupRules": {
                      "Message": {
                        "index": 1
                      },
                      "Slackbot": {
                        "index": 2
                      }
                    },
                    "data": {
                      "Ife16jY8bv": {
                        "id": "Ife16jY8bv",
                        "group": "parameters",
                        "key": "channel",
                        "value": {
                          "error": false,
                          "proxy": false,
                          "check": false,
                          "type": "string",
                          "collection": false,
                          "data": "C02B2FJ512P",
                          "available": []
                        },
                        "required": false,
                        "ref": false,
                        "metadata": {
                          "type": "dynamic",
                          "method": {
                            "channel": "slack",
                            "operation": "createChannelDropdown",
                            "key": "name",
                            "value": "id"
                          },
                          "displayname": "Channel",
                          "optional": false,
                          "ordering": 0,
                          "index": 0
                        },
                        "flags": "p"
                      },
                      "F2T2FPJI7S": {
                        "id": "F2T2FPJI7S",
                        "group": "parameters",
                        "key": "bot",
                        "value": {
                          "error": false,
                          "proxy": false,
                          "check": false,
                          "type": "string",
                          "collection": false,
                          "data": "Yes",
                          "available": []
                        },
                        "required": false,
                        "ref": false,
                        "metadata": {
                          "type": "list",
                          "displayname": "Send as bot?",
                          "choices": [
                            {
                              "label": "Yes",
                              "value": "Yes"
                            },
                            {
                              "label": "No",
                              "value": "No"
                            }
                          ],
                          "dependencies": [],
                          "optional": false,
                          "ordering": 1,
                          "index": 1
                        },
                        "flags": "p"
                      },
                      "TW-DVPAAdA": {
                        "id": "TW-DVPAAdA",
                        "group": "parameters",
                        "key": "links",
                        "value": {
                          "error": false,
                          "proxy": false,
                          "check": false,
                          "type": "string",
                          "collection": false,
                          "data": "Yes",
                          "available": []
                        },
                        "required": false,
                        "ref": false,
                        "metadata": {
                          "type": "list",
                          "displayname": "Unfurl URLs?",
                          "choices": [
                            {
                              "label": "Yes",
                              "value": "Yes"
                            },
                            {
                              "label": "No",
                              "value": "No"
                            }
                          ],
                          "dependencies": [],
                          "optional": false,
                          "ordering": 2,
                          "index": 2
                        },
                        "flags": "p"
                      },
                      "ZX_UAXJzcG": {
                        "id": "ZX_UAXJzcG",
                        "group": "parameters",
                        "key": "messageType",
                        "value": {
                          "error": false,
                          "proxy": false,
                          "check": false,
                          "type": "string",
                          "collection": false,
                          "data": "Plain Text",
                          "available": []
                        },
                        "required": false,
                        "ref": false,
                        "metadata": {
                          "type": "list",
                          "displayname": "Message Type",
                          "choices": [
                            {
                              "label": "Plain Text",
                              "value": "Plain Text"
                            },
                            {
                              "label": "Blocks",
                              "value": "Blocks"
                            }
                          ],
                          "dependencies": [],
                          "optional": false,
                          "ordering": 3,
                          "index": 3
                        },
                        "flags": "p"
                      },
                      "KzlQKseU9": {
                        "id": "KzlQKseU9",
                        "group": "Message",
                        "key": "Text",
                        "value": {
                          "error": false,
                          "proxy": false,
                          "check": false,
                          "type": "string",
                          "collection": false,
                          "data": "",
                          "available": [
                            "string"
                          ]
                        },
                        "required": true,
                        "ref": false,
                        "metadata": {
                          "index": 0,
                          "optional": false
                        },
                        "flags": "d"
                      },
                      "9l2k0p6n-H": {
                        "id": "9l2k0p6n-H",
                        "group": "Message",
                        "key": "Thread Timestamp",
                        "value": {
                          "error": false,
                          "proxy": false,
                          "check": false,
                          "type": "string",
                          "collection": false,
                          "data": "",
                          "available": [
                            "string"
                          ]
                        },
                        "required": false,
                        "ref": false,
                        "metadata": {
                          "index": 1,
                          "optional": false
                        },
                        "flags": "d"
                      },
                      "NJCwVK7J8k": {
                        "id": "NJCwVK7J8k",
                        "group": "Slackbot",
                        "key": "Name",
                        "value": {
                          "error": false,
                          "proxy": false,
                          "check": false,
                          "type": "string",
                          "collection": false,
                          "data": "",
                          "available": [
                            "string"
                          ]
                        },
                        "required": false,
                        "ref": false,
                        "metadata": {
                          "index": 0,
                          "optional": false
                        },
                        "flags": "d"
                      }
                    }
                  },
                  "outputs": {
                    "extensible": false,
                    "rules": {},
                    "groupRules": {
                      "Message": {
                        "extensible": false,
                        "reserved": {},
                        "index": 0,
                        "type": "object"
                      }
                    },
                    "data": {
                      "Z3jRv62Ahw": {
                        "id": "Z3jRv62Ahw",
                        "group": "Message",
                        "key": "Timestamp",
                        "value": {
                          "error": false,
                          "type": "string",
                          "collection": false,
                          "data": "",
                          "available": [
                            "string"
                          ]
                        },
                        "ref": false,
                        "metadata": {
                          "index": 0
                        }
                      }
                    }
                  },
                  "runtime": {},
                  "display": {},
                  "comments": "Send a message to a public or private channel as a user or bot in Slack.",
                  "enableNewMetadata": true
                }
              },
              "pins": {}
            },
            {
              "joins": {},
              "address": "root:kernel:control:0.0.1:callable",
              "parents": {
                "version": {
                  "address": "root:kernel:control:0.0.1",
                  "key": "0.0.1",
                  "data": {
                    "name": "0.0.1"
                  }
                },
                "channel": {
                  "address": "root:kernel:control",
                  "key": "control",
                  "data": {
                    "name": "control"
                  }
                }
              },
              "uuid": "I147q_jx-",
              "branches": {},
              "node": {
                "key": "callable",
                "data": {
                  "name": "Scheduled Flow"
                },
                "model": {
                  "type": "method",
                  "_v": 2,
                  "key": "callable",
                  "executable": false,
                  "displayed": true,
                  "async": false,
                  "cooperative": false,
                  "mirrored": true,
                  "inlined": false,
                  "dependencies": [],
                  "timeout": 30000,
                  "idempotent": false,
                  "monitor": false,
                  "webhook": false,
                  "webhookList": false,
                  "webhookConditions": false,
                  "mobile": false,
                  "hooks": {},
                  "policy": {
                    "error": {
                      "type": "finish"
                    }
                  },
                  "metadata": {
                    "id": null,
                    "name": "Scheduled Flow",
                    "description": "Start a Flow that executes on-demand, i.e. called by another Flow or via the Invoke API."
                  },
                  "meta": {},
                  "config": null,
                  "partnerChannelKeys": null,
                  "inputs": {
                    "extensible": true,
                    "rules": {
                      "*": {
                        "types": [
                          "*"
                        ],
                        "collection": "*"
                      }
                    },
                    "groupRules": {
                      "body": {
                        "type": "object",
                        "reserved": {},
                        "extensible": true
                      },
                      "headers": {
                        "type": "object",
                        "reserved": {
                          "Content-Type": "string"
                        },
                        "extensible": true
                      },
                      "query": {
                        "type": "object",
                        "reserved": {},
                        "extensible": true
                      }
                    },
                    "data": {
                      "gwa4kUs45U": {
                        "id": "gwa4kUs45U",
                        "group": "context",
                        "key": "execution_time",
                        "value": {
                          "error": false,
                          "type": "string",
                          "collection": false,
                          "data": null,
                          "available": []
                        },
                        "ref": false,
                        "metadata": {
                          "displayname": "Current Time ",
                          "index": 0
                        },
                        "required": false,
                        "flags": "d"
                      },
                      "IN4vIiiL2S": {
                        "id": "IN4vIiiL2S",
                        "group": "context",
                        "key": "execution_id",
                        "value": {
                          "error": false,
                          "type": "string",
                          "collection": false,
                          "data": null,
                          "available": []
                        },
                        "ref": false,
                        "metadata": {
                          "displayname": "Execution ID",
                          "index": 1
                        },
                        "required": false,
                        "flags": "d"
                      }
                    }
                  },
                  "outputs": {
                    "extensible": true,
                    "rules": {
                      "*": {
                        "types": [
                          "*"
                        ],
                        "collection": "*"
                      }
                    },
                    "data": {
                      "APxUA7NV5J": {
                        "id": "APxUA7NV5J",
                        "group": "context",
                        "key": "execution_time",
                        "value": {
                          "error": false,
                          "type": "string",
                          "collection": false,
                          "data": null,
                          "available": []
                        },
                        "ref": false,
                        "metadata": {
                          "displayname": "Current Time ",
                          "index": 0
                        }
                      },
                      "N4PNDKAqaw": {
                        "id": "N4PNDKAqaw",
                        "group": "context",
                        "key": "execution_id",
                        "value": {
                          "error": false,
                          "type": "string",
                          "collection": false,
                          "data": null,
                          "available": []
                        },
                        "ref": false,
                        "metadata": {
                          "displayname": "Execution ID",
                          "index": 1
                        }
                      }
                    },
                    "groupRules": {
                      "context": {
                        "extensible": false
                      },
                      "null": {
                        "extensible": false
                      }
                    }
                  },
                  "runtime": {}
                }
              },
              "pins": {}
            }
          ],
          "model": {},
          "orderings": {
            "EFLC8lpAoK": [
              "I147q_jx-",
              "Ys-ri8GzO"
            ],
            "ETYx4xa0x2": [
              "Ys-ri8GzO",
              "Euo2yu8PV"
            ],
            "hurIBv_sha": [
              "Euo2yu8PV",
              "4GEkrYQKY"
            ]
          },
          "cron": {
            "seconds": "00",
            "minutes": "0",
            "hours": "1",
            "dayOfTheMonth": "*",
            "month": "*",
            "dayOfTheWeek": "3,6",
            "startDate": "",
            "endDate": "",
            "recurrence": 0,
            "timeZone": "America/New_York"
          },
          "security_level": null,
          "log": true,
          "inheritLog": true,
          "scheduled": true,
          "group": "926046e9-c74d-4c6c-8411-cf697142e5bc",
          "templateName": null,
          "connector_method_meta": {
            "inputs": {},
            "outputs": {},
            "options": {}
          },
          "monitor_flo": false
        }
      }
    },
    "configs": {
      "e62cbc79-d44e-4a95-b9e1-e97f19fe6aad": {
        "id": "e62cbc79-d44e-4a95-b9e1-e97f19fe6aad",
        "name": "Slack Sandbox",
        "module": "slack",
        "data": null
      }
    },
    "tables": {},
    "groups": {
      "926046e9-c74d-4c6c-8411-cf697142e5bc": {
        "id": "926046e9-c74d-4c6c-8411-cf697142e5bc",
        "data": {
          "name": "Flows backup",
          "description": "",
          "media_uri": ""
        }
      }
    }
  }
}