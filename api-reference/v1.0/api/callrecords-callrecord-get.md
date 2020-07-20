---
title: 获取 callRecord
description: 检索 callrecord 对象的属性和关系。
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: ae239cd7bb559d8fc46cbaa43933a54d6ffe5e1c
ms.sourcegitcommit: 566d09c17f9d641b6fac9b9159405a3cc41e037b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/20/2020
ms.locfileid: "45183650"
---
# <a name="get-callrecord"></a><span data-ttu-id="648d0-103">获取 callRecord</span><span class="sxs-lookup"><span data-stu-id="648d0-103">Get callRecord</span></span>

<span data-ttu-id="648d0-104">命名空间：microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="648d0-104">Namespace: microsoft.graph.callRecords</span></span>

<span data-ttu-id="648d0-105">检索[callRecord](../resources/callrecords-callrecord.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="648d0-105">Retrieve the properties and relationships of a [callRecord](../resources/callrecords-callrecord.md) object.</span></span>

<span data-ttu-id="648d0-106">有两种方法可以获取**callRecord**的**id** ：</span><span class="sxs-lookup"><span data-stu-id="648d0-106">There are two ways to get the **id** of a **callRecord**:</span></span>

* <span data-ttu-id="648d0-107">订阅对终结点的[更改通知](/graph/api/resources/webhooks?view=graph-rest-1.0) `/communications/callRecords` 。</span><span class="sxs-lookup"><span data-stu-id="648d0-107">Subscribe to [change notifications](/graph/api/resources/webhooks?view=graph-rest-1.0) to the `/communications/callRecords` endpoint.</span></span>
* <span data-ttu-id="648d0-108">使用[调用](../resources/call.md)的**callChainId**属性。</span><span class="sxs-lookup"><span data-stu-id="648d0-108">Use the **callChainId** property of a [call](../resources/call.md).</span></span> <span data-ttu-id="648d0-109">只有在关联的呼叫完成后，呼叫记录才可用。</span><span class="sxs-lookup"><span data-stu-id="648d0-109">The call record is available only after the associated call is completed.</span></span>

## <a name="permissions"></a><span data-ttu-id="648d0-110">Permissions</span><span class="sxs-lookup"><span data-stu-id="648d0-110">Permissions</span></span>

<span data-ttu-id="648d0-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="648d0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="648d0-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="648d0-113">Permission type</span></span>                        | <span data-ttu-id="648d0-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="648d0-114">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="648d0-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="648d0-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="648d0-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="648d0-116">Not supported.</span></span> |
| <span data-ttu-id="648d0-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="648d0-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="648d0-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="648d0-118">Not supported.</span></span> |
| <span data-ttu-id="648d0-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="648d0-119">Application</span></span>                            | <span data-ttu-id="648d0-120">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="648d0-120">CallRecords.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="648d0-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="648d0-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /communications/callRecords/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="648d0-122">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="648d0-122">Optional query parameters</span></span>

<span data-ttu-id="648d0-123">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="648d0-123">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="648d0-124">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="648d0-124">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="648d0-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="648d0-125">Request headers</span></span>

| <span data-ttu-id="648d0-126">名称</span><span class="sxs-lookup"><span data-stu-id="648d0-126">Name</span></span>      |<span data-ttu-id="648d0-127">说明</span><span class="sxs-lookup"><span data-stu-id="648d0-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="648d0-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="648d0-128">Authorization</span></span> | <span data-ttu-id="648d0-129">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="648d0-129">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="648d0-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="648d0-130">Request body</span></span>

<span data-ttu-id="648d0-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="648d0-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="648d0-132">响应</span><span class="sxs-lookup"><span data-stu-id="648d0-132">Response</span></span>

<span data-ttu-id="648d0-133">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和请求的[callRecords callRecord](../resources/callrecords-callrecord.md)对象。</span><span class="sxs-lookup"><span data-stu-id="648d0-133">If successful, this method returns a `200 OK` response code and the requested [microsoft.graph.callRecords.callRecord](../resources/callrecords-callrecord.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="648d0-134">示例</span><span class="sxs-lookup"><span data-stu-id="648d0-134">Examples</span></span>

### <a name="example-1-get-basic-details"></a><span data-ttu-id="648d0-135">示例1：获取基本详细信息</span><span class="sxs-lookup"><span data-stu-id="648d0-135">Example 1: Get basic details</span></span>

#### <a name="request"></a><span data-ttu-id="648d0-136">请求</span><span class="sxs-lookup"><span data-stu-id="648d0-136">Request</span></span>

<span data-ttu-id="648d0-137">下面的示例演示了从[callRecord](../resources/callrecords-callrecord.md)获取基本详细信息的请求。</span><span class="sxs-lookup"><span data-stu-id="648d0-137">The following is an example of the request to get the basic details from a [callRecord](../resources/callrecords-callrecord.md).</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_callrecord"
}-->

```http
GET https://graph.microsoft.com/v1.0/communications/callRecords/{id}
```

#### <a name="response"></a><span data-ttu-id="648d0-138">响应</span><span class="sxs-lookup"><span data-stu-id="648d0-138">Response</span></span>

<span data-ttu-id="648d0-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="648d0-139">The following is an example of the response.</span></span>

> <span data-ttu-id="648d0-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="648d0-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.callRecords.callRecord"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#communications/callRecords/$entity",
    "version": 1,
    "type": "peerToPeer",
    "modalities": [
        "audio"
    ],
    "lastModifiedDateTime": "2020-02-25T19:00:24.582757Z",
    "startDateTime": "2020-02-25T18:52:21.2169889Z",
    "endDateTime": "2020-02-25T18:52:46.7640013Z",
    "id": "e523d2ed-2966-4b6b-925b-754a88034cc5",
    "organizer": {
        "user": {
            "id": "821809f5-0000-0000-0000-3b5136c0e777",
            "displayName": "Abbie Wilkins",
            "tenantId": "dc368399-474c-4d40-900c-6265431fd81f"
        }
    },
    "participants": [
        {
            "user": {
                "id": "821809f5-0000-0000-0000-3b5136c0e777",
                "displayName": "Abbie Wilkins",
                "tenantId": "dc368399-474c-4d40-900c-6265431fd81f"
            }
        },
        {
            "user": {
                "id": "f69e2c00-0000-0000-0000-185e5f5f5d8a",
                "displayName": "Owen Franklin",
                "tenantId": "dc368399-474c-4d40-900c-6265431fd81f"
            }
        }
    ]
}
```

### <a name="example-2-get-full-details"></a><span data-ttu-id="648d0-142">示例2：获取完整详细信息</span><span class="sxs-lookup"><span data-stu-id="648d0-142">Example 2: Get full details</span></span>

#### <a name="request"></a><span data-ttu-id="648d0-143">请求</span><span class="sxs-lookup"><span data-stu-id="648d0-143">Request</span></span>

<span data-ttu-id="648d0-144">下面是从[callRecord](../resources/callrecords-callrecord.md)中获取完整详细信息（包括会话和分段组件）的请求示例。</span><span class="sxs-lookup"><span data-stu-id="648d0-144">The following is an example of the request to get the full details from a [callRecord](../resources/callrecords-callrecord.md), including session and segment components.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_callrecord_expanded"
}-->

```http
GET https://graph.microsoft.com/v1.0/communications/callRecords/{id}?$expand=sessions($expand=segments)
```

#### <a name="response"></a><span data-ttu-id="648d0-145">响应</span><span class="sxs-lookup"><span data-stu-id="648d0-145">Response</span></span>

<span data-ttu-id="648d0-146">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="648d0-146">The following is an example of the response.</span></span> <span data-ttu-id="648d0-147">如果 "会话" 列表被截断， `sessions@odata.nextlink` 将提供一个值，以检索下一个会话页面。</span><span class="sxs-lookup"><span data-stu-id="648d0-147">If the sessions list is truncated, a `sessions@odata.nextlink` value will be provided to retrieve the next page of sessions.</span></span>

> <span data-ttu-id="648d0-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="648d0-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.callRecords.callRecord"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#communications/callRecords(sessions(segments()))/$entity",
    "version": 1,
    "type": "peerToPeer",
    "modalities": [
        "audio"
    ],
    "lastModifiedDateTime": "2020-02-25T19:00:24.582757Z",
    "startDateTime": "2020-02-25T18:52:21.2169889Z",
    "endDateTime": "2020-02-25T18:52:46.7640013Z",
    "id": "e523d2ed-2966-4b6b-925b-754a88034cc5",
    "organizer": {
        "user": {
            "id": "821809f5-0000-0000-0000-3b5136c0e777",
            "displayName": "Abbie Wilkins",
            "tenantId": "dc368399-474c-4d40-900c-6265431fd81f"
        }
    },
    "participants": [
        {
            "user": {
                "id": "821809f5-0000-0000-0000-3b5136c0e777",
                "displayName": "Abbie Wilkins",
                "tenantId": "dc368399-474c-4d40-900c-6265431fd81f"
            }
        },
        {
            "user": {
                "id": "f69e2c00-0000-0000-0000-185e5f5f5d8a",
                "displayName": "Owen Franklin",
                "tenantId": "dc368399-474c-4d40-900c-6265431fd81f"
            }
        }
    ],
    "sessions@odata.context": "https://graph.microsoft.com/v1.0/$metadata#communications/callRecords('e523d2ed-2966-4b6b-925b-754a88034cc5')/sessions(segments())",
    "sessions": [
        {
            "modalities": [
                "audio"
            ],
            "startDateTime": "2020-02-25T18:52:21.2169889Z",
            "endDateTime": "2020-02-25T18:52:46.7640013Z",
            "id": "e523d2ed-2966-4b6b-925b-754a88034cc5",
            "caller": {
                "@odata.type": "#microsoft.graph.callRecords.participantEndpoint",
                "userAgent": {
                    "@odata.type": "#microsoft.graph.callRecords.clientUserAgent",
                    "headerValue": "RTCC/7.0.0.0 UCWA/7.0.0.0 AndroidLync/6.25.0.27 (SM-G930U Android 8.0.0)",
                    "platform": "android",
                    "productFamily": "skypeForBusiness"
                },
                "identity": {
                    "@odata.type": "#microsoft.graph.identitySet",
                    "user": {
                        "id": "821809f5-0000-0000-0000-3b5136c0e777",
                        "displayName": "Abbie Wilkins",
                        "tenantId": "dc368399-474c-4d40-900c-6265431fd81f"
                    }
                }
            },
            "callee": {
                "@odata.type": "#microsoft.graph.callRecords.participantEndpoint",
                "userAgent": {
                    "@odata.type": "#microsoft.graph.callRecords.clientUserAgent",
                    "headerValue": "UCCAPI/16.0.12527.20122 OC/16.0.12527.20194 (Skype for Business)",
                    "platform": "windows",
                    "productFamily": "skypeForBusiness"
                },
                "identity": {
                    "user": {
                        "id": "f69e2c00-0000-0000-0000-185e5f5f5d8a",
                        "displayName": "Owen Franklin",
                        "tenantId": "dc368399-474c-4d40-900c-6265431fd81f"
                    }
                },
                "feedback": {
                    "rating": "poor",
                    "tokens": {
                        "NoSound": false,
                        "OtherNoSound": false,
                        "Echo": false,
                        "Noisy": true,
                        "LowVolume": false,
                        "Stopped": false,
                        "DistortedSound": false,
                        "Interruptions": false
                    }
                }
            },
            "segments@odata.context": "https://graph.microsoft.com/v1.0/$metadata#communications/callRecords('e523d2ed-2966-4b6b-925b-754a88034cc5')/sessions('e523d2ed-2966-4b6b-925b-754a88034cc5')/segments",
            "segments": [
                {
                    "startDateTime": "2020-02-25T18:52:21.2169889Z",
                    "endDateTime": "2020-02-25T18:52:46.7640013Z",
                    "id": "e523d2ed-2966-4b6b-925b-754a88034cc5",
                    "caller": {
                        "@odata.type": "#microsoft.graph.callRecords.participantEndpoint",
                        "userAgent": {
                            "@odata.type": "#microsoft.graph.callRecords.clientUserAgent",
                            "headerValue": "RTCC/7.0.0.0 UCWA/7.0.0.0 AndroidLync/6.25.0.27 (SM-G930U Android 8.0.0)",
                            "platform": "android",
                            "productFamily": "skypeForBusiness"
                        },
                        "identity": {
                            "user": {
                                "id": "821809f5-0000-0000-0000-3b5136c0e777",
                                "displayName": "Abbie Wilkins",
                                "tenantId": "dc368399-474c-4d40-900c-6265431fd81f"
                            }
                        }
                    },
                    "callee": {
                        "@odata.type": "#microsoft.graph.callRecords.participantEndpoint",
                        "userAgent": {
                            "@odata.type": "#microsoft.graph.callRecords.clientUserAgent",
                            "headerValue": "UCCAPI/16.0.12527.20122 OC/16.0.12527.20194 (Skype for Business)",
                            "platform": "windows",
                            "productFamily": "skypeForBusiness"
                        },
                        "identity": {
                            "user": {
                                "id": "f69e2c00-0000-0000-0000-185e5f5f5d8a",
                                "displayName": "Owen Franklin",
                                "tenantId": "dc368399-474c-4d40-900c-6265431fd81f"
                            }
                        }
                    },
                    "media": [
                        {
                            "label": "main-audio",
                            "callerNetwork": {
                                "ipAddress": "10.150.0.2",
                                "subnet": "10.150.0.0",
                                "linkSpeed": 54000000,
                                "connectionType": "wifi",
                                "port": 27288,
                                "reflexiveIPAddress": "127.0.0.2",
                                "relayIPAddress": "52.114.188.32",
                                "relayPort": 53889,
                                "macAddress": "00-00-00-00-00-00",
                                "dnsSuffix": null,
                                "sentQualityEventRatio": 0,
                                "receivedQualityEventRatio": 0.27,
                                "delayEventRatio": 0,
                                "bandwidthLowEventRatio": 0
                            },
                            "calleeNetwork": {
                                "ipAddress": "10.139.0.12",
                                "subnet": "10.139.80.0",
                                "linkSpeed": 4294967295,
                                "connectionType": "wired",
                                "port": 50011,
                                "reflexiveIPAddress": "127.0.0.2",
                                "relayIPAddress": "52.114.188.102",
                                "relayPort": 52810,
                                "macAddress": "00-00-00-00-00-00-00-00",
                                "dnsSuffix": null,
                                "sentQualityEventRatio": 0.31,
                                "receivedQualityEventRatio": 0,
                                "delayEventRatio": 0,
                                "bandwidthLowEventRatio": 0
                            },
                            "callerDevice": {
                                "captureDeviceName": "Default input device",
                                "renderDeviceName": "Default output device",
                                "receivedSignalLevel": -10,
                                "receivedNoiseLevel": -68,
                                "initialSignalLevelRootMeanSquare": 60.25816,
                                "renderZeroVolumeEventRatio": 1,
                                "renderMuteEventRatio": 1,
                                "micGlitchRate": 23,
                                "speakerGlitchRate": 3830
                            },
                            "calleeDevice": {
                                "captureDeviceName": "Microphone (Microsoft Virtual Audio Device (Simple) (WDM))",
                                "captureDeviceDriver": "Microsoft: 5.0.8638.1100",
                                "renderDeviceName": "Speakers (Microsoft Virtual Audio Device (Simple) (WDM))",
                                "renderDeviceDriver": "Microsoft: 5.0.8638.1100",
                                "receivedSignalLevel": -14,
                                "receivedNoiseLevel": -86,
                                "initialSignalLevelRootMeanSquare": 146.7885,
                                "micGlitchRate": 143,
                                "speakerGlitchRate": 182
                            },
                            "streams": [
                                {
                                    "streamId": "1504545584",
                                    "streamDirection": "callerToCallee",
                                    "averageAudioDegradation": null,
                                    "averageJitter": "PT0.016S",
                                    "maxJitter": "PT0.021S",
                                    "averagePacketLossRate": 0,
                                    "maxPacketLossRate": 0,
                                    "averageRatioOfConcealedSamples": null,
                                    "maxRatioOfConcealedSamples": null,
                                    "averageRoundTripTime": "PT0.061S",
                                    "maxRoundTripTime": "PT0.079S",
                                    "packetUtilization": 67,
                                    "averageBandwidthEstimate": 9965083,
                                    "wasMediaBypassed": false,
                                    "averageAudioNetworkJitter": "PT0.043S",
                                    "maxAudioNetworkJitter": "PT0.046S"
                                },
                                {
                                    "streamId": "1785122252",
                                    "streamDirection": "calleeToCaller",
                                    "averageAudioDegradation": 1.160898,
                                    "averageJitter": "PT0.007S",
                                    "maxJitter": "PT0.012S",
                                    "averagePacketLossRate": 0.01381693,
                                    "maxPacketLossRate": 0.03738318,
                                    "averageRatioOfConcealedSamples": 0.06233422,
                                    "maxRatioOfConcealedSamples": 0.07192807,
                                    "averageRoundTripTime": "PT0.064S",
                                    "maxRoundTripTime": "PT0.106S",
                                    "packetUtilization": 709,
                                    "averageBandwidthEstimate": 15644878,
                                    "wasMediaBypassed": false,
                                    "averageAudioNetworkJitter": "PT0.266S",
                                    "maxAudioNetworkJitter": "PT0.474S"
                                }
                            ]
                        }
                    ]
                }
            ]
        }
    ],
    "sessions@odata.nextlink": "https://graph.microsoft.com/v1.0/$metadata#communications/callRecords('e523d2ed-2966-4b6b-925b-754a88034cc5')/sessions?$expand=segments&$skiptoken=abc"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get callRecord",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
