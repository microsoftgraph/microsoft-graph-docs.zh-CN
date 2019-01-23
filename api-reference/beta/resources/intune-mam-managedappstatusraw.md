---
title: managedAppStatusRaw 资源类型
description: 表示有关组织应用保护和配置的非类型化状态报告。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: bfc7815e7f893294a72b88f67054702e1fb7347e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399260"
---
# <a name="managedappstatusraw-resource-type"></a><span data-ttu-id="180bf-103">managedAppStatusRaw 资源类型</span><span class="sxs-lookup"><span data-stu-id="180bf-103">managedAppStatusRaw resource type</span></span>

> <span data-ttu-id="180bf-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="180bf-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="180bf-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="180bf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="180bf-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="180bf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="180bf-107">表示有关组织应用保护和配置的非类型化状态报告。</span><span class="sxs-lookup"><span data-stu-id="180bf-107">Represents an un-typed status report about organizations app protection and configuration.</span></span>


<span data-ttu-id="180bf-108">继承自 [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="180bf-108">Inherits from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>

## <a name="methods"></a><span data-ttu-id="180bf-109">方法</span><span class="sxs-lookup"><span data-stu-id="180bf-109">Methods</span></span>
|<span data-ttu-id="180bf-110">方法</span><span class="sxs-lookup"><span data-stu-id="180bf-110">Method</span></span>|<span data-ttu-id="180bf-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="180bf-111">Return Type</span></span>|<span data-ttu-id="180bf-112">说明</span><span class="sxs-lookup"><span data-stu-id="180bf-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="180bf-113">列出 managedAppStatusRaws</span><span class="sxs-lookup"><span data-stu-id="180bf-113">List managedAppStatusRaws</span></span>](../api/intune-mam-managedappstatusraw-list.md)|<span data-ttu-id="180bf-114">[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) 集合</span><span class="sxs-lookup"><span data-stu-id="180bf-114">[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) collection</span></span>|<span data-ttu-id="180bf-115">列出 [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="180bf-115">List properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) objects.</span></span>|
|[<span data-ttu-id="180bf-116">获取 managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="180bf-116">Get managedAppStatusRaw</span></span>](../api/intune-mam-managedappstatusraw-get.md)|[<span data-ttu-id="180bf-117">managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="180bf-117">managedAppStatusRaw</span></span>](../resources/intune-mam-managedappstatusraw.md)|<span data-ttu-id="180bf-118">读取 [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="180bf-118">Read properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="180bf-119">属性</span><span class="sxs-lookup"><span data-stu-id="180bf-119">Properties</span></span>
|<span data-ttu-id="180bf-120">属性</span><span class="sxs-lookup"><span data-stu-id="180bf-120">Property</span></span>|<span data-ttu-id="180bf-121">类型</span><span class="sxs-lookup"><span data-stu-id="180bf-121">Type</span></span>|<span data-ttu-id="180bf-122">说明</span><span class="sxs-lookup"><span data-stu-id="180bf-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="180bf-123">displayName</span><span class="sxs-lookup"><span data-stu-id="180bf-123">displayName</span></span>|<span data-ttu-id="180bf-124">String</span><span class="sxs-lookup"><span data-stu-id="180bf-124">String</span></span>|<span data-ttu-id="180bf-125">状态报告的友好名称。</span><span class="sxs-lookup"><span data-stu-id="180bf-125">Friendly name of the status report.</span></span> <span data-ttu-id="180bf-126">继承自 [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="180bf-126">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="180bf-127">id</span><span class="sxs-lookup"><span data-stu-id="180bf-127">id</span></span>|<span data-ttu-id="180bf-128">String</span><span class="sxs-lookup"><span data-stu-id="180bf-128">String</span></span>|<span data-ttu-id="180bf-129">实体的键。</span><span class="sxs-lookup"><span data-stu-id="180bf-129">Key of the entity.</span></span> <span data-ttu-id="180bf-130">继承自 [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="180bf-130">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="180bf-131">version</span><span class="sxs-lookup"><span data-stu-id="180bf-131">version</span></span>|<span data-ttu-id="180bf-132">String</span><span class="sxs-lookup"><span data-stu-id="180bf-132">String</span></span>|<span data-ttu-id="180bf-133">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="180bf-133">Version of the entity.</span></span> <span data-ttu-id="180bf-134">继承自 [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="180bf-134">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="180bf-135">content</span><span class="sxs-lookup"><span data-stu-id="180bf-135">content</span></span>|[<span data-ttu-id="180bf-136">Json</span><span class="sxs-lookup"><span data-stu-id="180bf-136">Json</span></span>](../resources/intune-mam-json.md)|<span data-ttu-id="180bf-137">状态报告内容。</span><span class="sxs-lookup"><span data-stu-id="180bf-137">Status report content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="180bf-138">关系</span><span class="sxs-lookup"><span data-stu-id="180bf-138">Relationships</span></span>
<span data-ttu-id="180bf-139">无</span><span class="sxs-lookup"><span data-stu-id="180bf-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="180bf-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="180bf-140">JSON Representation</span></span>
<span data-ttu-id="180bf-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="180bf-141">Here is a JSON representation of the resource.</span></span>
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




