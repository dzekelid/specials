{
  "info": {
    "name": "Foursquare Post Specials Retire",
    "_postman_id": "ce34f7fd-d044-4f9c-a091-bf7633edc5be",
    "description": "/specials/{ID}/flag",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Campaigns",
      "item": [
        {
          "id": "1a2e51ca-719a-4049-90d2-ba6047e09f43",
          "name": "campaignscampaign-id",
          "request": {
            "url": "http://api.foursquare.com/v2/campaigns/add?campaignId=%7B%7D&endAt=%7B%7D&groupId=%7B%7D&specialId=%7B%7D&startAt=%7B%7D&v=%7B%7D&venueId=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/campaigns/{CAMPAIGN_ID}"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "11b1e0d5-b09c-4e92-9a57-80c99a23474d"
            }
          ]
        },
        {
          "id": "ae392828-fa55-40d2-92d6-d3c88b75e1f9",
          "name": "campaignsadd",
          "request": {
            "url": "http://api.foursquare.com/v2/campaigns/list?groupId=%7B%7D&specialId=%7B%7D&status=%7B%7D&v=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/campaigns/add"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "058f5b71-5c99-42e3-8384-7a9060d69507"
            }
          ]
        },
        {
          "id": "6d2fbe5d-154c-4d42-b6a4-66045a09891e",
          "name": "specialsspecial-idretire",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "campaigns/:CAMPAIGN_ID"
              ],
              "query": [
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "CAMPAIGN_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/specials/{SPECIAL_ID}/retire"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fa442a8e-db9e-472e-8380-7d1e4f72c758"
            }
          ]
        },
        {
          "id": "14bb5894-a133-488c-b809-819bb6b6f66d",
          "name": "campaignscampaign-idtimeseries",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "campaigns/:CAMPAIGN_ID/delete"
              ],
              "query": [
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "CAMPAIGN_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/campaigns/{CAMPAIGN_ID}/timeseries"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7f707b60-6b7b-41d2-81f6-70e96c58fa5c"
            }
          ]
        },
        {
          "id": "94c86dac-ff3b-4366-bcbf-8777e026c077",
          "name": "campaignscampaign-iddelete",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "campaigns/:CAMPAIGN_ID/end"
              ],
              "query": [
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "CAMPAIGN_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/campaigns/{CAMPAIGN_ID}/delete"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7d142ab7-0ee7-4bdf-b93f-c44104f7495f"
            }
          ]
        },
        {
          "id": "156ec928-26af-4c3e-aa87-c8631ab65bca",
          "name": "campaignscampaign-idend",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "campaigns/:CAMPAIGN_ID/start"
              ],
              "query": [
                {
                  "key": "startAt",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "CAMPAIGN_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/campaigns/{CAMPAIGN_ID}/end"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a7d3fc8b-3eed-4742-bb08-6449d612d059"
            }
          ]
        },
        {
          "id": "3aa9112b-d82c-44ce-88a1-520c5711da6c",
          "name": "campaignslist",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "campaigns/:CAMPAIGN_ID/timeseries"
              ],
              "query": [
                {
                  "key": "endAt",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "startAt",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "CAMPAIGN_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/campaigns/list"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9ff66b00-9dd1-4d84-a99a-3208c4f0499c"
            }
          ]
        }
      ]
    },
    {
      "name": "Checkins",
      "item": [
        {
          "id": "5fc0e254-47aa-44c8-85b0-47b99d480fb8",
          "name": "checkinscheckin-id",
          "request": {
            "url": "http://api.foursquare.com/v2/checkins/add?alt=%7B%7D&altAcc=%7B%7D&broadcast=%7B%7D&eventId=%7B%7D&ll=%7B%7D&llAcc=%7B%7D&shout=%7B%7D&v=%7B%7D&venue=%7B%7D&venueId=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/checkins/{CHECKIN_ID}"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "79b5adda-2e88-4356-afa8-0551960f2b1a"
            }
          ]
        },
        {
          "id": "7f28289e-f5e0-473b-9cb1-ddb703230ea9",
          "name": "checkinsadd",
          "request": {
            "url": "http://api.foursquare.com/v2/checkins/recent?afterTimestamp=%7B%7D&limit=%7B%7D&ll=%7B%7D&v=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/checkins/add"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "256c7ae3-1506-4300-b0d5-f8c307a3cfcf"
            }
          ]
        },
        {
          "id": "60c363da-1936-4f63-b47f-bb91c9365594",
          "name": "venuegroupsgroup-idremovevenue",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "checkins/:CHECKIN_ID"
              ],
              "query": [
                {
                  "key": "signature",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "CHECKIN_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/venuegroups/{GROUP_ID}/removevenue"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a5d89a67-d194-41c0-97d1-664a9320a1ff"
            }
          ]
        },
        {
          "id": "fa50f7e0-caa6-49ed-9c50-69ba2ae1dd9a",
          "name": "checkinsrecent",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "checkins/:CHECKIN_ID/addcomment"
              ],
              "query": [
                {
                  "key": "text",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "CHECKIN_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/checkins/recent"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5d2b5e08-3594-435e-94c0-abe75ffb4ef2"
            }
          ]
        },
        {
          "id": "9f091d62-e9ad-48f0-b6a4-4cfc580a419a",
          "name": "checkinscheckin-idaddcomment",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "checkins/:CHECKIN_ID/deletecomment"
              ],
              "query": [
                {
                  "key": "commentId",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "CHECKIN_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/checkins/{CHECKIN_ID}/addcomment"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5e303fdb-0fd0-4288-b1ec-59c4ff18ee99"
            }
          ]
        }
      ]
    },
    {
      "name": "Events",
      "item": [
        {
          "id": "d96e71d1-7ee8-4bac-9d6b-f2be89ec1d55",
          "name": "eventsevent-id",
          "request": {
            "url": "http://api.foursquare.com/v2/events/categories?v=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/events/{EVENT_ID}"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8cc66987-0d92-4d23-bce2-280a6b80d490"
            }
          ]
        },
        {
          "id": "ec2a5bbf-4ffb-4afb-b2b1-e91b925400ef",
          "name": "eventscategories",
          "request": {
            "url": "http://api.foursquare.com/v2/events/search?domain=%7B%7D&eventId=%7B%7D&participantId=%7B%7D&v=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/events/categories"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4b131301-2ae8-4b67-a114-b56b221a03c1"
            }
          ]
        },
        {
          "id": "f481d838-46f0-4dfa-9128-2b9cb825f4ed",
          "name": "campaignscampaign-idstart",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "events/:EVENT_ID"
              ],
              "query": [
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "EVENT_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/campaigns/{CAMPAIGN_ID}/start"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fc684453-4ef5-4eeb-a5a5-b0ea0970f22f"
            }
          ]
        }
      ]
    },
    {
      "name": "Lists",
      "item": [
        {
          "id": "9b37a377-ebf4-4302-ad0d-9da39b023aa7",
          "name": "listslist-id",
          "request": {
            "url": "http://api.foursquare.com/v2/lists/add?collaborative=%7B%7D&description=%7B%7D&name=%7B%7D&photoId=%7B%7D&v=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/lists/{LIST_ID}"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9806993d-81ef-4ddd-a7af-049a1e0d3475"
            }
          ]
        },
        {
          "id": "4984f329-b876-4a5d-bdf2-67c532c8413d",
          "name": "tipstip-idunmark",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "lists/:LIST_ID"
              ],
              "query": [
                {
                  "key": "limit",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "offset",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "LIST_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/tips/{TIP_ID}/unmark"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f8129cfd-e201-4c4f-8662-62dbf07941c6"
            }
          ]
        },
        {
          "id": "5b8021b8-da6f-4af9-a54a-31daae50e0b5",
          "name": "listslist-idsuggestvenues",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "lists/:LIST_ID/additem"
              ],
              "query": [
                {
                  "key": "itemId",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "listId",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "text",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "tipId",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "url",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "venueId",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "LIST_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/lists/{LIST_ID}/suggestvenues"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "42ae831d-abe9-48f4-b53d-de637e8e00d6"
            }
          ]
        },
        {
          "id": "f0b04799-cfec-44fb-a84b-36e49616f862",
          "name": "listslist-idadditem",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "lists/:LIST_ID/deleteitem"
              ],
              "query": [
                {
                  "key": "itemId",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "LIST_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/lists/{LIST_ID}/additem"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "beaa6deb-d81a-49fd-8a8a-9eaf94996051"
            }
          ]
        },
        {
          "id": "30c295b9-78b7-45f2-a194-a03f15a8bcd1",
          "name": "listslist-iddeleteitem",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "lists/:LIST_ID/follow"
              ],
              "query": [
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "LIST_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/lists/{LIST_ID}/deleteitem"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f1128e51-9848-44b5-8a56-83f0dc79cd87"
            }
          ]
        },
        {
          "id": "44611492-55c1-4f94-ad44-5e77cdc19769",
          "name": "listsadd",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "lists/:LIST_ID/followers"
              ],
              "query": [
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "LIST_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/lists/add"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4885f928-be99-436f-a913-9a5e607992f0"
            }
          ]
        },
        {
          "id": "c24e0988-9108-44b4-b059-1b8459fc01c2",
          "name": "listslist-idfollow",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "lists/:LIST_ID/moveitem"
              ],
              "query": [
                {
                  "key": "afterId",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "beforeId",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "itemId",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "LIST_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/lists/{LIST_ID}/follow"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "159a7030-48c1-459e-b6b9-768772018540"
            }
          ]
        },
        {
          "id": "51febe3c-a3bc-4912-aa41-4067b2f904f3",
          "name": "listslist-idmoveitem",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "lists/:LIST_ID/share"
              ],
              "query": [
                {
                  "key": "broadcast",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "message",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "LIST_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/lists/{LIST_ID}/moveitem"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fd0fc000-47fc-4de0-a85f-b495e336ec3c"
            }
          ]
        },
        {
          "id": "0b698932-01a4-4d94-9bd1-c744910e326c",
          "name": "listslist-idfollowers",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "lists/:LIST_ID/suggestphoto"
              ],
              "query": [
                {
                  "key": "itemId",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "LIST_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/lists/{LIST_ID}/followers"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "eca969eb-2a39-4a4d-8d02-d9bb61b834ab"
            }
          ]
        },
        {
          "id": "e0404b4c-31d4-4fee-9a15-7eb0c725cbda",
          "name": "listslist-idsuggestphoto",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "lists/:LIST_ID/suggesttip"
              ],
              "query": [
                {
                  "key": "itemId",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "LIST_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/lists/{LIST_ID}/suggestphoto"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "aec4c3d5-49b2-4023-a707-255f5499dfd4"
            }
          ]
        },
        {
          "id": "6c3eba36-41e3-4043-930f-5f1b84ced2da",
          "name": "listslist-idsuggesttip",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "lists/:LIST_ID/suggestvenues"
              ],
              "query": [
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "LIST_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/lists/{LIST_ID}/suggesttip"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f3737062-0462-4c8e-bdc8-bd4948c1ced4"
            }
          ]
        },
        {
          "id": "1dfe7078-f668-4f78-a23d-cca6e2f33199",
          "name": "listslist-idshare",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "lists/:LIST_ID/unfollow"
              ],
              "query": [
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "LIST_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/lists/{LIST_ID}/share"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "708404e9-eaf0-46cc-b312-e4c56bde1ea3"
            }
          ]
        },
        {
          "id": "34631c54-6fc2-4465-9b3b-336a6ca36805",
          "name": "listslist-idunfollow",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "lists/:LIST_ID/update"
              ],
              "query": [
                {
                  "key": "collaborative",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "description",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "name",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "photoId",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "LIST_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/lists/{LIST_ID}/unfollow"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a03390d2-e0f1-47fb-85b1-06953199e120"
            }
          ]
        },
        {
          "id": "f198df2a-b8c2-44be-9801-e5b7b34f7541",
          "name": "listslist-idupdate",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "lists/:LIST_ID/updateitem"
              ],
              "query": [
                {
                  "key": "itemId",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "photoId",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "text",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "tipId",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "url",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "LIST_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/lists/{LIST_ID}/update"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2a4bc6f3-9274-4fb9-bf15-dd9f57ec4e81"
            }
          ]
        }
      ]
    },
    {
      "name": "Multi",
      "item": [
        {
          "id": "b799e1c6-3c2a-4dfc-8d81-20ecb5506c4e",
          "name": "pagespage-idvenues",
          "request": {
            "url": "http://api.foursquare.com/v2/multi?requests=%7B%7D&v=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/pages/{PAGE_ID}/venues"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8570e0c9-3087-4876-81fe-d5a167f37c89"
            }
          ]
        }
      ]
    },
    {
      "name": "Pages",
      "item": [
        {
          "id": "e6aa9b95-53c4-4e53-8d84-459121d2eeb1",
          "name": "pagespage-id",
          "request": {
            "url": "http://api.foursquare.com/v2/pages/search?fbid=%7B%7D&name=%7B%7D&twitter=%7B%7D&v=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/pages/{PAGE_ID}"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a3bce337-9d8b-461a-a763-a9ce87589075"
            }
          ]
        },
        {
          "id": "1339bb49-6504-4684-9bc1-28a009097756",
          "name": "eventssearch",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "pages/:PAGE_ID"
              ],
              "query": [
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "PAGE_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/events/search"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a2f6b7cb-6d80-4372-a3d3-98ef17dfe8c1"
            }
          ]
        },
        {
          "id": "7c158a34-533a-41b6-9b32-d6684a21bab9",
          "name": "pagessearch",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "pages/:PAGE_ID/venues"
              ],
              "query": [
                {
                  "key": "limit",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "ll",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "ne",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "offset",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "radius",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "sw",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "PAGE_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/pages/search"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d281e56b-5c48-4ae8-be8e-1387f002913e"
            }
          ]
        }
      ]
    },
    {
      "name": "Photos",
      "item": [
        {
          "id": "e6b0f19a-1a75-4f07-b376-b72545e839d6",
          "name": "photosphoto-id",
          "request": {
            "url": "http://api.foursquare.com/v2/photos/add?alt=%7B%7D&altAcc=%7B%7D&broadcast=%7B%7D&checkinId=%7B%7D&Content-Type=%7B%7D&image=%7B%7D&ll=%7B%7D&llAcc=%7B%7D&public=%7B%7D&tipId=%7B%7D&v=%7B%7D&venueId=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/photos/{PHOTO_ID}"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3fa9ec05-2d8e-403e-a395-422d62c42f3f"
            }
          ]
        },
        {
          "id": "a18191a1-4062-4751-998a-902394aef546",
          "name": "updatesmarknotificationsread",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "photos/:PHOTO_ID"
              ],
              "query": [
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "PHOTO_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/updates/marknotificationsread"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c3677ef5-4d4f-46d4-ac7f-ecbaa73e4aa9"
            }
          ]
        }
      ]
    },
    {
      "name": "Settings",
      "item": [
        {
          "id": "992d88f1-225f-43d3-8693-4c98a8f95610",
          "name": "settingssetting-id",
          "request": {
            "url": "http://api.foursquare.com/v2/settings/all?v=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/settings/{SETTING_ID}"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "060121be-4e81-4572-8d7e-0ab9bab95932"
            }
          ]
        },
        {
          "id": "2b67a319-ed2d-4d5f-a95e-cffda57b49c0",
          "name": "photosadd",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "settings/:SETTING_ID"
              ],
              "query": [
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "SETTING_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/photos/add"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4bec81ce-f195-4d1f-8af4-a4f0c9956529"
            }
          ]
        },
        {
          "id": "852a28b0-d662-44b5-b578-d84db864455a",
          "name": "settingsall",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "settings/:SETTING_ID/set"
              ],
              "query": [
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "value",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "SETTING_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/settings/all"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1805ffac-4217-4253-8a59-063c6383fbb5"
            }
          ]
        }
      ]
    },
    {
      "name": "Specials",
      "item": [
        {
          "id": "963ca9b5-7c8d-4c23-b76a-dc0148669e44",
          "name": "specialsspecial-id",
          "request": {
            "url": "http://api.foursquare.com/v2/specials/add?cost=%7B%7D&count1=%7B%7D&count2=%7B%7D&count3=%7B%7D&finePrint=%7B%7D&name=%7B%7D&offerId=%7B%7D&text=%7B%7D&type=%7B%7D&unlockedText=%7B%7D&v=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/specials/{SPECIAL_ID}"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "475e2829-dc2a-41d9-8856-7750dcc8802d"
            }
          ]
        },
        {
          "id": "722efb5b-7506-427c-8768-b628acf545ab",
          "name": "specialsadd",
          "request": {
            "url": "http://api.foursquare.com/v2/specials/list?status=%7B%7D&v=%7B%7D&venueId=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/specials/add"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ced31381-ce2e-4261-961f-3408489cba32"
            }
          ]
        },
        {
          "id": "a00c57e2-38c6-415d-bfeb-d61f4d4c8278",
          "name": "specialslist",
          "request": {
            "url": "http://api.foursquare.com/v2/specials/search?alt=%7B%7D&altAcc=%7B%7D&limit=%7B%7D&ll=%7B%7D&llAcc=%7B%7D&radius=%7B%7D&v=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/specials/list"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "558aef7f-3008-40e9-bbeb-964d459ae0c8"
            }
          ]
        },
        {
          "id": "c5afca62-19b9-4ec0-99b3-f1941f8f60cc",
          "name": "specialsspecial-idconfiguration",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "specials/:ID/flag"
              ],
              "query": [
                {
                  "key": "problem",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "text",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "venueId",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/specials/{SPECIAL_ID}/configuration"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "519c7355-af94-4132-b37c-4bb2f006dbd5"
            }
          ]
        },
        {
          "id": "5ce1f97a-e004-4f26-8666-93b299e435ad",
          "name": "settingssetting-idset",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "specials/:SPECIAL_ID"
              ],
              "query": [
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "venueId",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "SPECIAL_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/settings/{SETTING_ID}/set"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "750af321-cffa-4595-93cf-3d03624e618c"
            }
          ]
        },
        {
          "id": "23e6196c-ef93-4928-8ffa-729030c9a6c8",
          "name": "specialssearch",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "specials/:SPECIAL_ID/configuration"
              ],
              "query": [
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "SPECIAL_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/specials/search"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5a44d579-9035-4261-b8a8-3d82ea3ad712"
            }
          ]
        },
        {
          "id": "a55e1a0b-59d8-4795-b8e1-515255c67d4e",
          "name": "specialsidflag",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.foursquare.com",
              "path": [
                "v2",
                "specials/:SPECIAL_ID/retire"
              ],
              "query": [
                {
                  "key": "v",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "SPECIAL_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/specials/{ID}/flag"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6e0694ff-208e-4623-92a9-b4d8e4a3f044"
            }
          ]
        }
      ]
    }
  ]
}