---
title: 获取 callRecord
description: 检索 callrecord 对象的属性和关系。
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: a770cfe7d30c3480e2e6a81dd3c8f9c10d480452
ms.sourcegitcommit: 43f7800894857a29f02fffaf4a50ad6386b5bf59
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/03/2020
ms.locfileid: "44524615"
---
# <a name="get-callrecord"></a><span data-ttu-id="fae0a-103">获取 callRecord</span><span class="sxs-lookup"><span data-stu-id="fae0a-103">Get callRecord</span></span>

<span data-ttu-id="fae0a-104">命名空间：microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="fae0a-104">Namespace: microsoft.graph.callRecords</span></span>

<span data-ttu-id="fae0a-105">检索[callRecord](../resources/callrecords-callrecord.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="fae0a-105">Retrieve the properties and relationships of a [callRecord](../resources/callrecords-callrecord.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="fae0a-106">权限</span><span class="sxs-lookup"><span data-stu-id="fae0a-106">Permissions</span></span>

<span data-ttu-id="fae0a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fae0a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fae0a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="fae0a-109">Permission type</span></span>                        | <span data-ttu-id="fae0a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fae0a-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="fae0a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fae0a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="fae0a-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="fae0a-112">Not supported.</span></span> |
| <span data-ttu-id="fae0a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fae0a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fae0a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="fae0a-114">Not supported.</span></span> |
| <span data-ttu-id="fae0a-115">Application</span><span class="sxs-lookup"><span data-stu-id="fae0a-115">Application</span></span>                            | <span data-ttu-id="fae0a-116">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="fae0a-116">CallRecords.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fae0a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fae0a-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /communications/callRecords/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fae0a-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="fae0a-118">Optional query parameters</span></span>

<span data-ttu-id="fae0a-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="fae0a-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="fae0a-120">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="fae0a-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="fae0a-121">请求头</span><span class="sxs-lookup"><span data-stu-id="fae0a-121">Request headers</span></span>

| <span data-ttu-id="fae0a-122">名称</span><span class="sxs-lookup"><span data-stu-id="fae0a-122">Name</span></span>      |<span data-ttu-id="fae0a-123">说明</span><span class="sxs-lookup"><span data-stu-id="fae0a-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="fae0a-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="fae0a-124">Authorization</span></span> | <span data-ttu-id="fae0a-125">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="fae0a-125">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="fae0a-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="fae0a-126">Request body</span></span>

<span data-ttu-id="fae0a-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="fae0a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fae0a-128">响应</span><span class="sxs-lookup"><span data-stu-id="fae0a-128">Response</span></span>

<span data-ttu-id="fae0a-129">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和请求的[callRecords callRecord](../resources/callrecords-callrecord.md)对象。</span><span class="sxs-lookup"><span data-stu-id="fae0a-129">If successful, this method returns a `200 OK` response code and the requested [microsoft.graph.callRecords.callRecord](../resources/callrecords-callrecord.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fae0a-130">示例</span><span class="sxs-lookup"><span data-stu-id="fae0a-130">Examples</span></span>

### <a name="example-1-get-basic-details"></a><span data-ttu-id="fae0a-131">示例1：获取基本详细信息</span><span class="sxs-lookup"><span data-stu-id="fae0a-131">Example 1: Get basic details</span></span>

#### <a name="request"></a><span data-ttu-id="fae0a-132">请求</span><span class="sxs-lookup"><span data-stu-id="fae0a-132">Request</span></span>

<span data-ttu-id="fae0a-133">下面的示例演示了从[callRecord](../resources/callrecords-callrecord.md)获取基本详细信息的请求。</span><span class="sxs-lookup"><span data-stu-id="fae0a-133">The following is an example of the request to get the basic details from a [callRecord](../resources/callrecords-callrecord.md).</span></span>


# <a name="http"></a>[<span data-ttu-id="fae0a-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="fae0a-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_callrecord"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/communications/callRecords/{id}
```
# <a name="c"></a>[<span data-ttu-id="fae0a-135">C#</span><span class="sxs-lookup"><span data-stu-id="fae0a-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-callrecord-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fae0a-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fae0a-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-callrecord-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fae0a-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fae0a-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-callrecord-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fae0a-138">Java</span><span class="sxs-lookup"><span data-stu-id="fae0a-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-callrecord-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="fae0a-139">响应</span><span class="sxs-lookup"><span data-stu-id="fae0a-139">Response</span></span>

<span data-ttu-id="fae0a-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="fae0a-140">The following is an example of the response.</span></span>

> <span data-ttu-id="fae0a-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="fae0a-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
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

### <a name="example-2-get-full-details"></a><span data-ttu-id="fae0a-143">示例2：获取完整详细信息</span><span class="sxs-lookup"><span data-stu-id="fae0a-143">Example 2: Get full details</span></span>

#### <a name="request"></a><span data-ttu-id="fae0a-144">请求</span><span class="sxs-lookup"><span data-stu-id="fae0a-144">Request</span></span>

<span data-ttu-id="fae0a-145">下面是从[callRecord](../resources/callrecords-callrecord.md)中获取完整详细信息（包括会话和分段组件）的请求示例。</span><span class="sxs-lookup"><span data-stu-id="fae0a-145">The following is an example of the request to get the full details from a [callRecord](../resources/callrecords-callrecord.md), including session and segment components.</span></span>


# <a name="http"></a>[<span data-ttu-id="fae0a-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="fae0a-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_callrecord_expanded"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/communications/callRecords/{id}?$expand=sessions($expand=segments)
```
# <a name="c"></a>[<span data-ttu-id="fae0a-147">C#</span><span class="sxs-lookup"><span data-stu-id="fae0a-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-callrecord-expanded-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fae0a-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fae0a-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-callrecord-expanded-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fae0a-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fae0a-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-callrecord-expanded-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fae0a-150">Java</span><span class="sxs-lookup"><span data-stu-id="fae0a-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-callrecord-expanded-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="fae0a-151">响应</span><span class="sxs-lookup"><span data-stu-id="fae0a-151">Response</span></span>

<span data-ttu-id="fae0a-152">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="fae0a-152">The following is an example of the response.</span></span> <span data-ttu-id="fae0a-153">如果 "会话" 列表被截断， `sessions@odata.nextlink` 将提供一个值，以检索下一个会话页面。</span><span class="sxs-lookup"><span data-stu-id="fae0a-153">If the sessions list is truncated, a `sessions@odata.nextlink` value will be provided to retrieve the next page of sessions.</span></span>

> <span data-ttu-id="fae0a-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="fae0a-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
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
