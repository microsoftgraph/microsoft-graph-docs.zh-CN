---
title: managedAppStatusRaw 资源类型
description: 表示有关组织应用保护和配置的非类型化状态报告。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c89b36f7b9587a99d280de789dcaa753442591e9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32465235"
---
# <a name="managedappstatusraw-resource-type"></a><span data-ttu-id="1efd7-103">managedAppStatusRaw 资源类型</span><span class="sxs-lookup"><span data-stu-id="1efd7-103">managedAppStatusRaw resource type</span></span>

> <span data-ttu-id="1efd7-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1efd7-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1efd7-105">表示有关组织应用保护和配置的非类型化状态报告。</span><span class="sxs-lookup"><span data-stu-id="1efd7-105">Represents an un-typed status report about organizations app protection and configuration.</span></span>


<span data-ttu-id="1efd7-106">继承自 [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="1efd7-106">Inherits from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>

## <a name="methods"></a><span data-ttu-id="1efd7-107">方法</span><span class="sxs-lookup"><span data-stu-id="1efd7-107">Methods</span></span>
|<span data-ttu-id="1efd7-108">方法</span><span class="sxs-lookup"><span data-stu-id="1efd7-108">Method</span></span>|<span data-ttu-id="1efd7-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="1efd7-109">Return Type</span></span>|<span data-ttu-id="1efd7-110">说明</span><span class="sxs-lookup"><span data-stu-id="1efd7-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1efd7-111">列出 managedAppStatusRaws</span><span class="sxs-lookup"><span data-stu-id="1efd7-111">List managedAppStatusRaws</span></span>](../api/intune-mam-managedappstatusraw-list.md)|<span data-ttu-id="1efd7-112">[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1efd7-112">[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) collection</span></span>|<span data-ttu-id="1efd7-113">列出 [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1efd7-113">List properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) objects.</span></span>|
|[<span data-ttu-id="1efd7-114">获取 managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="1efd7-114">Get managedAppStatusRaw</span></span>](../api/intune-mam-managedappstatusraw-get.md)|[<span data-ttu-id="1efd7-115">managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="1efd7-115">managedAppStatusRaw</span></span>](../resources/intune-mam-managedappstatusraw.md)|<span data-ttu-id="1efd7-116">读取 [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1efd7-116">Read properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="1efd7-117">属性</span><span class="sxs-lookup"><span data-stu-id="1efd7-117">Properties</span></span>
|<span data-ttu-id="1efd7-118">属性</span><span class="sxs-lookup"><span data-stu-id="1efd7-118">Property</span></span>|<span data-ttu-id="1efd7-119">类型</span><span class="sxs-lookup"><span data-stu-id="1efd7-119">Type</span></span>|<span data-ttu-id="1efd7-120">说明</span><span class="sxs-lookup"><span data-stu-id="1efd7-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1efd7-121">displayName</span><span class="sxs-lookup"><span data-stu-id="1efd7-121">displayName</span></span>|<span data-ttu-id="1efd7-122">String</span><span class="sxs-lookup"><span data-stu-id="1efd7-122">String</span></span>|<span data-ttu-id="1efd7-123">状态报告的友好名称。</span><span class="sxs-lookup"><span data-stu-id="1efd7-123">Friendly name of the status report.</span></span> <span data-ttu-id="1efd7-124">继承自 [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="1efd7-124">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="1efd7-125">id</span><span class="sxs-lookup"><span data-stu-id="1efd7-125">id</span></span>|<span data-ttu-id="1efd7-126">String</span><span class="sxs-lookup"><span data-stu-id="1efd7-126">String</span></span>|<span data-ttu-id="1efd7-127">实体的键。</span><span class="sxs-lookup"><span data-stu-id="1efd7-127">Key of the entity.</span></span> <span data-ttu-id="1efd7-128">继承自 [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="1efd7-128">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="1efd7-129">version</span><span class="sxs-lookup"><span data-stu-id="1efd7-129">version</span></span>|<span data-ttu-id="1efd7-130">String</span><span class="sxs-lookup"><span data-stu-id="1efd7-130">String</span></span>|<span data-ttu-id="1efd7-131">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="1efd7-131">Version of the entity.</span></span> <span data-ttu-id="1efd7-132">继承自 [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="1efd7-132">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="1efd7-133">content</span><span class="sxs-lookup"><span data-stu-id="1efd7-133">content</span></span>|[<span data-ttu-id="1efd7-134">Json</span><span class="sxs-lookup"><span data-stu-id="1efd7-134">Json</span></span>](../resources/intune-mam-json.md)|<span data-ttu-id="1efd7-135">状态报告内容。</span><span class="sxs-lookup"><span data-stu-id="1efd7-135">Status report content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1efd7-136">关系</span><span class="sxs-lookup"><span data-stu-id="1efd7-136">Relationships</span></span>
<span data-ttu-id="1efd7-137">无</span><span class="sxs-lookup"><span data-stu-id="1efd7-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1efd7-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1efd7-138">JSON Representation</span></span>
<span data-ttu-id="1efd7-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1efd7-139">Here is a JSON representation of the resource.</span></span>
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



