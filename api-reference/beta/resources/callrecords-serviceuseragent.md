---
title: serviceUserAgent 资源类型
description: ServiceUserAgent 类型
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 9cf6b0483ebda33068824f0a3345c12894fd2d7e
ms.sourcegitcommit: ef9e0fd8fb6047fa9272e98310eaed2c4e0a2660
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/23/2020
ms.locfileid: "44353118"
---
# <a name="serviceuseragent-resource-type"></a><span data-ttu-id="8b8ec-103">serviceUserAgent 资源类型</span><span class="sxs-lookup"><span data-stu-id="8b8ec-103">serviceUserAgent resource type</span></span>

<span data-ttu-id="8b8ec-104">命名空间：microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="8b8ec-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8b8ec-105">表示呼叫中终结点的服务用户代理。</span><span class="sxs-lookup"><span data-stu-id="8b8ec-105">Represents a service user agent of an endpoint in a call.</span></span> <span data-ttu-id="8b8ec-106">继承自[userAgent](callrecords-useragent.md)类型。</span><span class="sxs-lookup"><span data-stu-id="8b8ec-106">Inherits from [userAgent](callrecords-useragent.md) type.</span></span>

## <a name="properties"></a><span data-ttu-id="8b8ec-107">属性</span><span class="sxs-lookup"><span data-stu-id="8b8ec-107">Properties</span></span>

| <span data-ttu-id="8b8ec-108">属性</span><span class="sxs-lookup"><span data-stu-id="8b8ec-108">Property</span></span>     | <span data-ttu-id="8b8ec-109">类型</span><span class="sxs-lookup"><span data-stu-id="8b8ec-109">Type</span></span>        | <span data-ttu-id="8b8ec-110">说明</span><span class="sxs-lookup"><span data-stu-id="8b8ec-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8b8ec-111">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="8b8ec-111">applicationVersion</span></span>|<span data-ttu-id="8b8ec-112">String</span><span class="sxs-lookup"><span data-stu-id="8b8ec-112">String</span></span>|<span data-ttu-id="8b8ec-113">标识此终结点使用的应用程序软件的版本。</span><span class="sxs-lookup"><span data-stu-id="8b8ec-113">Identifies the version of application software used by this endpoint.</span></span>|
|<span data-ttu-id="8b8ec-114">headerValue</span><span class="sxs-lookup"><span data-stu-id="8b8ec-114">headerValue</span></span>|<span data-ttu-id="8b8ec-115">字符串</span><span class="sxs-lookup"><span data-stu-id="8b8ec-115">String</span></span>|<span data-ttu-id="8b8ec-116">此终结点报告的用户代理标头值。</span><span class="sxs-lookup"><span data-stu-id="8b8ec-116">User-agent header value reported by this endpoint.</span></span>|
|<span data-ttu-id="8b8ec-117">role</span><span class="sxs-lookup"><span data-stu-id="8b8ec-117">role</span></span>|<span data-ttu-id="8b8ec-118">callRecords。 serviceRole</span><span class="sxs-lookup"><span data-stu-id="8b8ec-118">microsoft.graph.callRecords.serviceRole</span></span>|<span data-ttu-id="8b8ec-119">标识此终结点使用的服务的角色。</span><span class="sxs-lookup"><span data-stu-id="8b8ec-119">Identifies the role of the service used by this endpoint.</span></span> <span data-ttu-id="8b8ec-120">可取值为：`unknown`、`customBot`、`skypeForBusinessMicrosoftTeamsGateway`、`skypeForBusinessAudioVideoMcu`、`skypeForBusinessApplicationSharingMcu`、`skypeForBusinessCallQueues`、`skypeForBusinessAutoAttendant`、`mediationServer`、`mediationServerCloudConnectorEdition`、`exchangeUnifiedMessagingService`、`mediaController`、`conferencingAnnouncementService`、`conferencingAttendant`、`audioTeleconferencerController`、`skypeForBusinessUnifiedCommunicationApplicationPlatform`、`responseGroupServiceAnnouncementService`、`gateway`、`skypeTranslator`、`skypeForBusinessAttendant`、`responseGroupService`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="8b8ec-120">Possible values are: `unknown`, `customBot`, `skypeForBusinessMicrosoftTeamsGateway`, `skypeForBusinessAudioVideoMcu`, `skypeForBusinessApplicationSharingMcu`, `skypeForBusinessCallQueues`, `skypeForBusinessAutoAttendant`, `mediationServer`, `mediationServerCloudConnectorEdition`, `exchangeUnifiedMessagingService`, `mediaController`, `conferencingAnnouncementService`, `conferencingAttendant`, `audioTeleconferencerController`, `skypeForBusinessUnifiedCommunicationApplicationPlatform`, `responseGroupServiceAnnouncementService`, `gateway`, `skypeTranslator`, `skypeForBusinessAttendant`, `responseGroupService`, `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8b8ec-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8b8ec-121">JSON representation</span></span>

<span data-ttu-id="8b8ec-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8b8ec-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.serviceUserAgent",
  "baseType": "microsoft.graph.callRecords.userAgent"
}-->

```json
{
  "applicationVersion": "String",
  "headerValue": "String",
  "role": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "serviceUserAgent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->