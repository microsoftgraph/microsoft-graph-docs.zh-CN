---
title: 获取 callRecord
description: 检索 callrecord 对象的属性和关系。
localization_priority: Normal
author: williamlooney
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 557fc6bf408b8536aad249474dbb248aa2c6f69d
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047586"
---
# <a name="get-callrecord"></a><span data-ttu-id="2c11b-103">获取 callRecord</span><span class="sxs-lookup"><span data-stu-id="2c11b-103">Get callRecord</span></span>

<span data-ttu-id="2c11b-104">命名空间：microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="2c11b-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2c11b-105">检索 [callRecord](../resources/callrecords-callrecord.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="2c11b-105">Retrieve the properties and relationships of a [callRecord](../resources/callrecords-callrecord.md) object.</span></span>

<span data-ttu-id="2c11b-106">有两种方法可以获取 **callRecord 的** **ID：**</span><span class="sxs-lookup"><span data-stu-id="2c11b-106">There are two ways to get the **id** of a **callRecord**:</span></span>

* <span data-ttu-id="2c11b-107">订阅 [终结点更改](/graph/api/resources/webhooks?view=graph-rest-beta) `/communications/callRecords` 通知。</span><span class="sxs-lookup"><span data-stu-id="2c11b-107">Subscribe to [change notifications](/graph/api/resources/webhooks?view=graph-rest-beta) to the `/communications/callRecords` endpoint.</span></span>
* <span data-ttu-id="2c11b-108">使用 **呼叫 的 callChainId** [属性](../resources/call.md)。</span><span class="sxs-lookup"><span data-stu-id="2c11b-108">Use the **callChainId** property of a [call](../resources/call.md).</span></span> <span data-ttu-id="2c11b-109">呼叫记录仅在关联的呼叫完成之后可用。</span><span class="sxs-lookup"><span data-stu-id="2c11b-109">The call record is available only after the associated call is completed.</span></span>

## <a name="permissions"></a><span data-ttu-id="2c11b-110">权限</span><span class="sxs-lookup"><span data-stu-id="2c11b-110">Permissions</span></span>

<span data-ttu-id="2c11b-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2c11b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2c11b-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="2c11b-113">Permission type</span></span>                        | <span data-ttu-id="2c11b-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2c11b-114">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="2c11b-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2c11b-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="2c11b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2c11b-116">Not supported.</span></span> |
| <span data-ttu-id="2c11b-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2c11b-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2c11b-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="2c11b-118">Not supported.</span></span> |
| <span data-ttu-id="2c11b-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="2c11b-119">Application</span></span>                            | <span data-ttu-id="2c11b-120">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="2c11b-120">CallRecords.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2c11b-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2c11b-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /communications/callRecords/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2c11b-122">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="2c11b-122">Optional query parameters</span></span>

<span data-ttu-id="2c11b-123">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="2c11b-123">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="2c11b-124">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="2c11b-124">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="2c11b-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="2c11b-125">Request headers</span></span>

| <span data-ttu-id="2c11b-126">名称</span><span class="sxs-lookup"><span data-stu-id="2c11b-126">Name</span></span>      |<span data-ttu-id="2c11b-127">说明</span><span class="sxs-lookup"><span data-stu-id="2c11b-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2c11b-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="2c11b-128">Authorization</span></span> | <span data-ttu-id="2c11b-129">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="2c11b-129">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="2c11b-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="2c11b-130">Request body</span></span>

<span data-ttu-id="2c11b-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2c11b-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2c11b-132">响应</span><span class="sxs-lookup"><span data-stu-id="2c11b-132">Response</span></span>

<span data-ttu-id="2c11b-133">如果成功，此方法在响应正文中返回 响应代码和请求的 `200 OK` [microsoft.graph.callRecords.callRecord](../resources/callrecords-callrecord.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2c11b-133">If successful, this method returns a `200 OK` response code and the requested [microsoft.graph.callRecords.callRecord](../resources/callrecords-callrecord.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2c11b-134">示例</span><span class="sxs-lookup"><span data-stu-id="2c11b-134">Examples</span></span>

### <a name="example-1-get-basic-details"></a><span data-ttu-id="2c11b-135">示例 1：获取基本详细信息</span><span class="sxs-lookup"><span data-stu-id="2c11b-135">Example 1: Get basic details</span></span>

#### <a name="request"></a><span data-ttu-id="2c11b-136">请求</span><span class="sxs-lookup"><span data-stu-id="2c11b-136">Request</span></span>

<span data-ttu-id="2c11b-137">下面是从 [callRecord](../resources/callrecords-callrecord.md)获取基本详细信息的请求示例。</span><span class="sxs-lookup"><span data-stu-id="2c11b-137">The following is an example of the request to get the basic details from a [callRecord](../resources/callrecords-callrecord.md).</span></span>


# <a name="http"></a>[<span data-ttu-id="2c11b-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="2c11b-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_callrecord"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/communications/callRecords/{id}
```
# <a name="c"></a>[<span data-ttu-id="2c11b-139">C#</span><span class="sxs-lookup"><span data-stu-id="2c11b-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-callrecord-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2c11b-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2c11b-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-callrecord-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2c11b-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2c11b-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-callrecord-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2c11b-142">Java</span><span class="sxs-lookup"><span data-stu-id="2c11b-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-callrecord-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2c11b-143">响应</span><span class="sxs-lookup"><span data-stu-id="2c11b-143">Response</span></span>

<span data-ttu-id="2c11b-144">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="2c11b-144">The following is an example of the response.</span></span>

> <span data-ttu-id="2c11b-145">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="2c11b-145">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.callRecords.callRecord"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#communications/callRecords/$entity",
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

### <a name="example-2-get-full-details"></a><span data-ttu-id="2c11b-146">示例 2：获取完整详细信息</span><span class="sxs-lookup"><span data-stu-id="2c11b-146">Example 2: Get full details</span></span>

#### <a name="request"></a><span data-ttu-id="2c11b-147">请求</span><span class="sxs-lookup"><span data-stu-id="2c11b-147">Request</span></span>

<span data-ttu-id="2c11b-148">下面是从 [callRecord](../resources/callrecords-callrecord.md)获取完整详细信息的请求示例，包括会话和分段组件。</span><span class="sxs-lookup"><span data-stu-id="2c11b-148">The following is an example of the request to get the full details from a [callRecord](../resources/callrecords-callrecord.md), including session and segment components.</span></span>


# <a name="http"></a>[<span data-ttu-id="2c11b-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="2c11b-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_callrecord_expanded"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/communications/callRecords/{id}?$expand=sessions($expand=segments)
```
# <a name="c"></a>[<span data-ttu-id="2c11b-150">C#</span><span class="sxs-lookup"><span data-stu-id="2c11b-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-callrecord-expanded-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2c11b-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2c11b-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-callrecord-expanded-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2c11b-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2c11b-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-callrecord-expanded-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2c11b-153">Java</span><span class="sxs-lookup"><span data-stu-id="2c11b-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-callrecord-expanded-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2c11b-154">响应</span><span class="sxs-lookup"><span data-stu-id="2c11b-154">Response</span></span>

<span data-ttu-id="2c11b-155">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="2c11b-155">The following is an example of the response.</span></span> <span data-ttu-id="2c11b-156">如果会话列表被截断，则会提供一个值 `sessions@odata.nextLink` 来检索下一页会话。</span><span class="sxs-lookup"><span data-stu-id="2c11b-156">If the sessions list is truncated, a `sessions@odata.nextLink` value will be provided to retrieve the next page of sessions.</span></span>

> <span data-ttu-id="2c11b-157">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="2c11b-157">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.callRecords.callRecord"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#communications/callRecords(sessions(segments()))/$entity",
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
    "sessions@odata.context": "https://graph.microsoft.com/beta/$metadata#communications/callRecords('e523d2ed-2966-4b6b-925b-754a88034cc5')/sessions(segments())",
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
    "sessions@odata.nextLink": "https://graph.microsoft.com/beta/$metadata#communications/callRecords('e523d2ed-2966-4b6b-925b-754a88034cc5')/sessions?$expand=segments&$skiptoken=abc"
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


