---
title: serviceAnnouncement 资源类型
description: 服务通信资源的顶级容器
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: resourcePageType
ms.openlocfilehash: c22cbcd9fd8e67137e649cc099ff7980468c246f
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2021
ms.locfileid: "53109099"
---
# <a name="serviceannouncement-resource-type"></a><span data-ttu-id="a3f9f-103">serviceAnnouncement 资源类型</span><span class="sxs-lookup"><span data-stu-id="a3f9f-103">serviceAnnouncement resource type</span></span>

<span data-ttu-id="a3f9f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a3f9f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a3f9f-105">服务通信资源的顶级容器。</span><span class="sxs-lookup"><span data-stu-id="a3f9f-105">A top-level container for service communications resources.</span></span>

## <a name="methods"></a><span data-ttu-id="a3f9f-106">方法</span><span class="sxs-lookup"><span data-stu-id="a3f9f-106">Methods</span></span>
|<span data-ttu-id="a3f9f-107">方法</span><span class="sxs-lookup"><span data-stu-id="a3f9f-107">Method</span></span>|<span data-ttu-id="a3f9f-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="a3f9f-108">Return type</span></span>|<span data-ttu-id="a3f9f-109">说明</span><span class="sxs-lookup"><span data-stu-id="a3f9f-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a3f9f-110">列出 healthOverviews</span><span class="sxs-lookup"><span data-stu-id="a3f9f-110">List healthOverviews</span></span>](../api/serviceannouncement-list-healthoverviews.md)|<span data-ttu-id="a3f9f-111">[serviceHealth](../resources/servicehealth.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a3f9f-111">[serviceHealth](../resources/servicehealth.md) collection</span></span>|<span data-ttu-id="a3f9f-112">从 healthOverviews 导航属性获取 serviceHealth 资源。</span><span class="sxs-lookup"><span data-stu-id="a3f9f-112">Get the serviceHealth resources from the healthOverviews navigation property.</span></span>|
|[<span data-ttu-id="a3f9f-113">列出问题</span><span class="sxs-lookup"><span data-stu-id="a3f9f-113">List issues</span></span>](../api/serviceannouncement-list-issues.md)|<span data-ttu-id="a3f9f-114">[serviceHealthIssue](../resources/servicehealthissue.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a3f9f-114">[serviceHealthIssue](../resources/servicehealthissue.md) collection</span></span>|<span data-ttu-id="a3f9f-115">从 issues 导航属性获取 serviceHealthIssue 资源。</span><span class="sxs-lookup"><span data-stu-id="a3f9f-115">Get the serviceHealthIssue resources from the issues navigation property.</span></span>|
|[<span data-ttu-id="a3f9f-116">列出邮件</span><span class="sxs-lookup"><span data-stu-id="a3f9f-116">List messages</span></span>](../api/serviceannouncement-list-messages.md)|<span data-ttu-id="a3f9f-117">[serviceUpdateMessage](../resources/serviceupdatemessage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a3f9f-117">[serviceUpdateMessage](../resources/serviceupdatemessage.md) collection</span></span>|<span data-ttu-id="a3f9f-118">从 messages 导航属性获取 serviceUpdateMessage 资源。</span><span class="sxs-lookup"><span data-stu-id="a3f9f-118">Get the serviceUpdateMessage resources from the messages navigation property.</span></span>|

## <a name="properties"></a><span data-ttu-id="a3f9f-119">属性</span><span class="sxs-lookup"><span data-stu-id="a3f9f-119">Properties</span></span>
<span data-ttu-id="a3f9f-120">无。</span><span class="sxs-lookup"><span data-stu-id="a3f9f-120">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="a3f9f-121">关系</span><span class="sxs-lookup"><span data-stu-id="a3f9f-121">Relationships</span></span>
|<span data-ttu-id="a3f9f-122">属性</span><span class="sxs-lookup"><span data-stu-id="a3f9f-122">Property</span></span>|<span data-ttu-id="a3f9f-123">类型</span><span class="sxs-lookup"><span data-stu-id="a3f9f-123">Type</span></span>|<span data-ttu-id="a3f9f-124">说明</span><span class="sxs-lookup"><span data-stu-id="a3f9f-124">Description</span></span>|
|-|-|-|
|<span data-ttu-id="a3f9f-125">messages</span><span class="sxs-lookup"><span data-stu-id="a3f9f-125">messages</span></span>|<span data-ttu-id="a3f9f-126">collection ([serviceUpdateMessage) ](serviceupdatemessage.md)</span><span class="sxs-lookup"><span data-stu-id="a3f9f-126">Collection([serviceUpdateMessage](serviceupdatemessage.md))</span></span>|<span data-ttu-id="a3f9f-127">租户的服务消息集合。</span><span class="sxs-lookup"><span data-stu-id="a3f9f-127">A collection of service messages for tenant.</span></span> <span data-ttu-id="a3f9f-128">此属性是包含的导航属性，可为空且可读。</span><span class="sxs-lookup"><span data-stu-id="a3f9f-128">This property is a contained navigation property, it is nullable and readonly.</span></span>|
|<span data-ttu-id="a3f9f-129">healthOverviews</span><span class="sxs-lookup"><span data-stu-id="a3f9f-129">healthOverviews</span></span>|<span data-ttu-id="a3f9f-130">collection ([serviceHealth](servicehealth.md)) </span><span class="sxs-lookup"><span data-stu-id="a3f9f-130">Collection([serviceHealth](servicehealth.md))</span></span>|<span data-ttu-id="a3f9f-131">租户的服务运行状况信息的集合。</span><span class="sxs-lookup"><span data-stu-id="a3f9f-131">A collection of service health information for tenant.</span></span> <span data-ttu-id="a3f9f-132">此属性是包含的导航属性，可为空且可读。</span><span class="sxs-lookup"><span data-stu-id="a3f9f-132">This property is a contained navigation property, it is nullable and readonly.</span></span>|
|<span data-ttu-id="a3f9f-133">问题</span><span class="sxs-lookup"><span data-stu-id="a3f9f-133">issues</span></span>|<span data-ttu-id="a3f9f-134">collection ([serviceHealthIssue) ](servicehealthissue.md)</span><span class="sxs-lookup"><span data-stu-id="a3f9f-134">Collection([serviceHealthIssue](servicehealthissue.md))</span></span>|<span data-ttu-id="a3f9f-135">租户的服务问题集合。</span><span class="sxs-lookup"><span data-stu-id="a3f9f-135">A collection of service issues for tenant.</span></span> <span data-ttu-id="a3f9f-136">此属性是包含的导航属性，可为空且可读。</span><span class="sxs-lookup"><span data-stu-id="a3f9f-136">This property is a contained navigation property, it is nullable and readonly.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a3f9f-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a3f9f-137">JSON representation</span></span>
<span data-ttu-id="a3f9f-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a3f9f-138">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.serviceAnnouncement",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.serviceAnnouncement"
}
```