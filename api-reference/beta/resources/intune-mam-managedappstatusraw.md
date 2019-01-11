---
title: managedAppStatusRaw 资源类型
description: 表示有关组织应用保护和配置的非类型化状态报告。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 975f43d064718b8457b40be707a54a0ea0eb69f7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884012"
---
# <a name="managedappstatusraw-resource-type"></a><span data-ttu-id="b3b03-103">managedAppStatusRaw 资源类型</span><span class="sxs-lookup"><span data-stu-id="b3b03-103">managedAppStatusRaw resource type</span></span>

> <span data-ttu-id="b3b03-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b3b03-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b3b03-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b3b03-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b3b03-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="b3b03-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b3b03-107">表示有关组织应用保护和配置的非类型化状态报告。</span><span class="sxs-lookup"><span data-stu-id="b3b03-107">Represents an un-typed status report about organizations app protection and configuration.</span></span>

<span data-ttu-id="b3b03-108">继承自 [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="b3b03-108">Inherits from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>

## <a name="methods"></a><span data-ttu-id="b3b03-109">方法</span><span class="sxs-lookup"><span data-stu-id="b3b03-109">Methods</span></span>
|<span data-ttu-id="b3b03-110">方法</span><span class="sxs-lookup"><span data-stu-id="b3b03-110">Method</span></span>|<span data-ttu-id="b3b03-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="b3b03-111">Return Type</span></span>|<span data-ttu-id="b3b03-112">说明</span><span class="sxs-lookup"><span data-stu-id="b3b03-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b3b03-113">列出 managedAppStatusRaws</span><span class="sxs-lookup"><span data-stu-id="b3b03-113">List managedAppStatusRaws</span></span>](../api/intune-mam-managedappstatusraw-list.md)|<span data-ttu-id="b3b03-114">[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b3b03-114">[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) collection</span></span>|<span data-ttu-id="b3b03-115">列出 [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b3b03-115">List properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) objects.</span></span>|
|[<span data-ttu-id="b3b03-116">获取 managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="b3b03-116">Get managedAppStatusRaw</span></span>](../api/intune-mam-managedappstatusraw-get.md)|[<span data-ttu-id="b3b03-117">managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="b3b03-117">managedAppStatusRaw</span></span>](../resources/intune-mam-managedappstatusraw.md)|<span data-ttu-id="b3b03-118">读取 [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b3b03-118">Read properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b3b03-119">属性</span><span class="sxs-lookup"><span data-stu-id="b3b03-119">Properties</span></span>
|<span data-ttu-id="b3b03-120">属性</span><span class="sxs-lookup"><span data-stu-id="b3b03-120">Property</span></span>|<span data-ttu-id="b3b03-121">类型</span><span class="sxs-lookup"><span data-stu-id="b3b03-121">Type</span></span>|<span data-ttu-id="b3b03-122">说明</span><span class="sxs-lookup"><span data-stu-id="b3b03-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b3b03-123">displayName</span><span class="sxs-lookup"><span data-stu-id="b3b03-123">displayName</span></span>|<span data-ttu-id="b3b03-124">String</span><span class="sxs-lookup"><span data-stu-id="b3b03-124">String</span></span>|<span data-ttu-id="b3b03-125">状态报告的友好名称。</span><span class="sxs-lookup"><span data-stu-id="b3b03-125">Friendly name of the status report.</span></span> <span data-ttu-id="b3b03-126">继承自 [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="b3b03-126">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="b3b03-127">id</span><span class="sxs-lookup"><span data-stu-id="b3b03-127">id</span></span>|<span data-ttu-id="b3b03-128">String</span><span class="sxs-lookup"><span data-stu-id="b3b03-128">String</span></span>|<span data-ttu-id="b3b03-129">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b3b03-129">Key of the entity.</span></span> <span data-ttu-id="b3b03-130">继承自 [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="b3b03-130">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="b3b03-131">version</span><span class="sxs-lookup"><span data-stu-id="b3b03-131">version</span></span>|<span data-ttu-id="b3b03-132">String</span><span class="sxs-lookup"><span data-stu-id="b3b03-132">String</span></span>|<span data-ttu-id="b3b03-133">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="b3b03-133">Version of the entity.</span></span> <span data-ttu-id="b3b03-134">继承自 [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="b3b03-134">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="b3b03-135">content</span><span class="sxs-lookup"><span data-stu-id="b3b03-135">content</span></span>|[<span data-ttu-id="b3b03-136">Json</span><span class="sxs-lookup"><span data-stu-id="b3b03-136">Json</span></span>](../resources/intune-mam-json.md)|<span data-ttu-id="b3b03-137">状态报告内容。</span><span class="sxs-lookup"><span data-stu-id="b3b03-137">Status report content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b3b03-138">关系</span><span class="sxs-lookup"><span data-stu-id="b3b03-138">Relationships</span></span>
<span data-ttu-id="b3b03-139">无</span><span class="sxs-lookup"><span data-stu-id="b3b03-139">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b3b03-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b3b03-140">JSON Representation</span></span>
<span data-ttu-id="b3b03-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b3b03-141">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppStatusRaw"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppStatusRaw",
  "displayName": "String",
  "id": "String (identifier)",
  "version": "String",
  "content": {
    "@odata.type": "microsoft.graph.Json"
  }
}
```





