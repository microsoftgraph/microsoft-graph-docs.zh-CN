---
title: serviceUserAgent 资源类型
description: ServiceUserAgent 类型
localization_priority: Normal
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 574fb733ad6d55a8cbdf36b8cf2de96bcaa8b8a6
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48601377"
---
# <a name="serviceuseragent-resource-type"></a><span data-ttu-id="ffdf6-103">serviceUserAgent 资源类型</span><span class="sxs-lookup"><span data-stu-id="ffdf6-103">serviceUserAgent resource type</span></span>

<span data-ttu-id="ffdf6-104">命名空间：microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="ffdf6-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ffdf6-105">表示呼叫中终结点的服务用户代理。</span><span class="sxs-lookup"><span data-stu-id="ffdf6-105">Represents a service user agent of an endpoint in a call.</span></span> <span data-ttu-id="ffdf6-106">继承自 [userAgent](callrecords-useragent.md) 类型。</span><span class="sxs-lookup"><span data-stu-id="ffdf6-106">Inherits from [userAgent](callrecords-useragent.md) type.</span></span>

## <a name="properties"></a><span data-ttu-id="ffdf6-107">属性</span><span class="sxs-lookup"><span data-stu-id="ffdf6-107">Properties</span></span>

| <span data-ttu-id="ffdf6-108">属性</span><span class="sxs-lookup"><span data-stu-id="ffdf6-108">Property</span></span>     | <span data-ttu-id="ffdf6-109">类型</span><span class="sxs-lookup"><span data-stu-id="ffdf6-109">Type</span></span>        | <span data-ttu-id="ffdf6-110">说明</span><span class="sxs-lookup"><span data-stu-id="ffdf6-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ffdf6-111">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="ffdf6-111">applicationVersion</span></span>|<span data-ttu-id="ffdf6-112">String</span><span class="sxs-lookup"><span data-stu-id="ffdf6-112">String</span></span>|<span data-ttu-id="ffdf6-113">标识此终结点使用的应用程序软件的版本。</span><span class="sxs-lookup"><span data-stu-id="ffdf6-113">Identifies the version of application software used by this endpoint.</span></span>|
|<span data-ttu-id="ffdf6-114">headerValue</span><span class="sxs-lookup"><span data-stu-id="ffdf6-114">headerValue</span></span>|<span data-ttu-id="ffdf6-115">String</span><span class="sxs-lookup"><span data-stu-id="ffdf6-115">String</span></span>|<span data-ttu-id="ffdf6-116">此终结点报告的用户代理标头值。</span><span class="sxs-lookup"><span data-stu-id="ffdf6-116">User-agent header value reported by this endpoint.</span></span>|
|<span data-ttu-id="ffdf6-117">role</span><span class="sxs-lookup"><span data-stu-id="ffdf6-117">role</span></span>|<span data-ttu-id="ffdf6-118">callRecords。 serviceRole</span><span class="sxs-lookup"><span data-stu-id="ffdf6-118">microsoft.graph.callRecords.serviceRole</span></span>|<span data-ttu-id="ffdf6-119">标识此终结点使用的服务的角色。</span><span class="sxs-lookup"><span data-stu-id="ffdf6-119">Identifies the role of the service used by this endpoint.</span></span> <span data-ttu-id="ffdf6-120">可能的值为：、、、、、、、、、、、、、、、、、、、、、 `unknown` `customBot` `skypeForBusinessMicrosoftTeamsGateway` `skypeForBusinessAudioVideoMcu` `skypeForBusinessApplicationSharingMcu` `skypeForBusinessCallQueues` `skypeForBusinessAutoAttendant` `mediationServer` `mediationServerCloudConnectorEdition` `exchangeUnifiedMessagingService` `mediaController` `conferencingAnnouncementService` `conferencingAttendant` `audioTeleconferencerController` `skypeForBusinessUnifiedCommunicationApplicationPlatform` `responseGroupServiceAnnouncementService` `gateway` `skypeTranslator` `skypeForBusinessAttendant` `responseGroupService` `voicemail` `unknownFutureValue` 。</span><span class="sxs-lookup"><span data-stu-id="ffdf6-120">Possible values are: `unknown`, `customBot`, `skypeForBusinessMicrosoftTeamsGateway`, `skypeForBusinessAudioVideoMcu`, `skypeForBusinessApplicationSharingMcu`, `skypeForBusinessCallQueues`, `skypeForBusinessAutoAttendant`, `mediationServer`, `mediationServerCloudConnectorEdition`, `exchangeUnifiedMessagingService`, `mediaController`, `conferencingAnnouncementService`, `conferencingAttendant`, `audioTeleconferencerController`, `skypeForBusinessUnifiedCommunicationApplicationPlatform`, `responseGroupServiceAnnouncementService`, `gateway`, `skypeTranslator`, `skypeForBusinessAttendant`, `responseGroupService`, `voicemail`, `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ffdf6-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ffdf6-121">JSON representation</span></span>

<span data-ttu-id="ffdf6-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ffdf6-122">The following is a JSON representation of the resource.</span></span>

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

