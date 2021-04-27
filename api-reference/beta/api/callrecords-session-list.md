---
title: 列出 callRecord 会话
description: 检索 callRecord 的会话对象列表。
localization_priority: Normal
author: williamlooney
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 2b575672befe470a6adfceb2a84ed1d22fe39d58
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047579"
---
# <a name="list-callrecord-sessions"></a><span data-ttu-id="1ad91-103">列出 callRecord 会话</span><span class="sxs-lookup"><span data-stu-id="1ad91-103">List callRecord sessions</span></span>

<span data-ttu-id="1ad91-104">命名空间：microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="1ad91-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1ad91-105">检索与[callRecord](../resources/callrecords-callrecord.md)对象关联的会话列表。 [](../resources/callrecords-session.md)</span><span class="sxs-lookup"><span data-stu-id="1ad91-105">Retrieve the list of [sessions](../resources/callrecords-session.md) associated with a [callRecord](../resources/callrecords-callrecord.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1ad91-106">权限</span><span class="sxs-lookup"><span data-stu-id="1ad91-106">Permissions</span></span>

<span data-ttu-id="1ad91-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1ad91-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1ad91-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="1ad91-109">Permission type</span></span>                        | <span data-ttu-id="1ad91-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1ad91-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1ad91-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1ad91-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1ad91-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="1ad91-112">Not supported.</span></span> |
| <span data-ttu-id="1ad91-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1ad91-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1ad91-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="1ad91-114">Not supported.</span></span> |
| <span data-ttu-id="1ad91-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="1ad91-115">Application</span></span>                            | <span data-ttu-id="1ad91-116">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="1ad91-116">CallRecords.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1ad91-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1ad91-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /communications/callRecords/{id}/sessions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1ad91-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="1ad91-118">Optional query parameters</span></span>

<span data-ttu-id="1ad91-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="1ad91-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="1ad91-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="1ad91-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="1ad91-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="1ad91-121">Request headers</span></span>

| <span data-ttu-id="1ad91-122">名称</span><span class="sxs-lookup"><span data-stu-id="1ad91-122">Name</span></span>      |<span data-ttu-id="1ad91-123">说明</span><span class="sxs-lookup"><span data-stu-id="1ad91-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1ad91-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="1ad91-124">Authorization</span></span> | <span data-ttu-id="1ad91-125">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="1ad91-125">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="1ad91-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="1ad91-126">Request body</span></span>

<span data-ttu-id="1ad91-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1ad91-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1ad91-128">响应</span><span class="sxs-lookup"><span data-stu-id="1ad91-128">Response</span></span>

<span data-ttu-id="1ad91-129">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和[](../resources/callrecords-session.md)请求的会话对象。</span><span class="sxs-lookup"><span data-stu-id="1ad91-129">If successful, this method returns a `200 OK` response code and the requested [session](../resources/callrecords-session.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1ad91-130">示例</span><span class="sxs-lookup"><span data-stu-id="1ad91-130">Examples</span></span>

### <a name="example-1-get-session-list"></a><span data-ttu-id="1ad91-131">示例 1：获取会话列表</span><span class="sxs-lookup"><span data-stu-id="1ad91-131">Example 1: Get session list</span></span>

#### <a name="request"></a><span data-ttu-id="1ad91-132">请求</span><span class="sxs-lookup"><span data-stu-id="1ad91-132">Request</span></span>

<span data-ttu-id="1ad91-133">下面是请求获取[callRecord](../resources/callrecords-callrecord.md)的[会话](../resources/callrecords-session.md)列表的示例。</span><span class="sxs-lookup"><span data-stu-id="1ad91-133">The following is an example of the request to get the list of [sessions](../resources/callrecords-session.md) for a [callRecord](../resources/callrecords-callrecord.md).</span></span>


# <a name="http"></a>[<span data-ttu-id="1ad91-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="1ad91-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_callrecord_sessions"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/communications/callRecords/{id}/sessions
```
# <a name="c"></a>[<span data-ttu-id="1ad91-135">C#</span><span class="sxs-lookup"><span data-stu-id="1ad91-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-callrecord-sessions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1ad91-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1ad91-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-callrecord-sessions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1ad91-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1ad91-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-callrecord-sessions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1ad91-138">Java</span><span class="sxs-lookup"><span data-stu-id="1ad91-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-callrecord-sessions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="1ad91-139">响应</span><span class="sxs-lookup"><span data-stu-id="1ad91-139">Response</span></span>

<span data-ttu-id="1ad91-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="1ad91-140">The following is an example of the response.</span></span>

> <span data-ttu-id="1ad91-141">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="1ad91-141">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.callRecords.session",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#communications/callRecords('e523d2ed-2966-4b6b-925b-754a88034cc5')/sessions",
    "value": [
        {
            "id": "e523d2ed-2966-4b6b-925b-754a88034cc5",
            "modalities": [
                "audio"
            ],
            "startDateTime": "2020-02-25T18:52:21.2169889Z",
            "endDateTime": "2020-02-25T18:52:46.7640013Z",
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
            }
        }
    ],
    "@odata.nextLink": "https://graph.microsoft.com/beta/$metadata#communications/callRecords('e523d2ed-2966-4b6b-925b-754a88034cc5')/sessions?$skiptoken=abc"
}
```

### <a name="example-2-get-session-list-with-segments"></a><span data-ttu-id="1ad91-142">示例 2：获取包含分段的会话列表</span><span class="sxs-lookup"><span data-stu-id="1ad91-142">Example 2: Get session list with segments</span></span>

#### <a name="request"></a><span data-ttu-id="1ad91-143">请求</span><span class="sxs-lookup"><span data-stu-id="1ad91-143">Request</span></span>

<span data-ttu-id="1ad91-144">下面是请求获取包含分段的[callRecord](../resources/callrecords-callrecord.md)的[](../resources/callrecords-session.md)会话[列表的示例。](../resources/callrecords-segment.md)</span><span class="sxs-lookup"><span data-stu-id="1ad91-144">The following is an example of the request to get the list of [sessions](../resources/callrecords-session.md) for a [callRecord](../resources/callrecords-callrecord.md) with [segments](../resources/callrecords-segment.md) included.</span></span>


# <a name="http"></a>[<span data-ttu-id="1ad91-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="1ad91-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_callrecord_sessions_expanded"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/communications/callRecords/{id}/sessions?$expand=segments
```
# <a name="c"></a>[<span data-ttu-id="1ad91-146">C#</span><span class="sxs-lookup"><span data-stu-id="1ad91-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-callrecord-sessions-expanded-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1ad91-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1ad91-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-callrecord-sessions-expanded-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1ad91-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1ad91-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-callrecord-sessions-expanded-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1ad91-149">Java</span><span class="sxs-lookup"><span data-stu-id="1ad91-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-callrecord-sessions-expanded-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="1ad91-150">响应</span><span class="sxs-lookup"><span data-stu-id="1ad91-150">Response</span></span>

<span data-ttu-id="1ad91-151">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="1ad91-151">The following is an example of the response.</span></span>

> <span data-ttu-id="1ad91-152">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="1ad91-152">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.callRecords.session",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#communications/callRecords('e523d2ed-2966-4b6b-925b-754a88034cc5')/sessions",
    "value": [
        {
            "id": "e523d2ed-2966-4b6b-925b-754a88034cc5",
            "modalities": [
                "audio"
            ],
            "startDateTime": "2020-02-25T18:52:21.2169889Z",
            "endDateTime": "2020-02-25T18:52:46.7640013Z",
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
            "segments@odata.context": "https://graph.microsoft.com/beta/$metadata#communications/callRecords('e523d2ed-2966-4b6b-925b-754a88034cc5')/sessions('e523d2ed-2966-4b6b-925b-754a88034cc5')/segments",
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
    "@odata.nextLink": "https://graph.microsoft.com/beta/$metadata#communications/callRecords('e523d2ed-2966-4b6b-925b-754a88034cc5')/sessions?$expand=segments&$skiptoken=abc"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List sessions",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


