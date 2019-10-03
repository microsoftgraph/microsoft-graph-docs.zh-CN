---
title: managedAppStatusRaw 资源类型
description: 表示有关组织应用保护和配置的非类型化状态报告。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4d6b597f23cc10ba27b57cf5acbe5baf8bc9c328
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37367012"
---
# <a name="managedappstatusraw-resource-type"></a><span data-ttu-id="51399-103">managedAppStatusRaw 资源类型</span><span class="sxs-lookup"><span data-stu-id="51399-103">managedAppStatusRaw resource type</span></span>

> <span data-ttu-id="51399-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="51399-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="51399-105">表示有关组织应用保护和配置的非类型化状态报告。</span><span class="sxs-lookup"><span data-stu-id="51399-105">Represents an un-typed status report about organizations app protection and configuration.</span></span>


<span data-ttu-id="51399-106">继承自 [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="51399-106">Inherits from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>

## <a name="methods"></a><span data-ttu-id="51399-107">方法</span><span class="sxs-lookup"><span data-stu-id="51399-107">Methods</span></span>
|<span data-ttu-id="51399-108">方法</span><span class="sxs-lookup"><span data-stu-id="51399-108">Method</span></span>|<span data-ttu-id="51399-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="51399-109">Return Type</span></span>|<span data-ttu-id="51399-110">说明</span><span class="sxs-lookup"><span data-stu-id="51399-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="51399-111">列出 managedAppStatusRaws</span><span class="sxs-lookup"><span data-stu-id="51399-111">List managedAppStatusRaws</span></span>](../api/intune-mam-managedappstatusraw-list.md)|<span data-ttu-id="51399-112">[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) 集合</span><span class="sxs-lookup"><span data-stu-id="51399-112">[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) collection</span></span>|<span data-ttu-id="51399-113">列出 [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="51399-113">List properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) objects.</span></span>|
|[<span data-ttu-id="51399-114">获取 managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="51399-114">Get managedAppStatusRaw</span></span>](../api/intune-mam-managedappstatusraw-get.md)|[<span data-ttu-id="51399-115">managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="51399-115">managedAppStatusRaw</span></span>](../resources/intune-mam-managedappstatusraw.md)|<span data-ttu-id="51399-116">读取 [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="51399-116">Read properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="51399-117">属性</span><span class="sxs-lookup"><span data-stu-id="51399-117">Properties</span></span>
|<span data-ttu-id="51399-118">属性</span><span class="sxs-lookup"><span data-stu-id="51399-118">Property</span></span>|<span data-ttu-id="51399-119">类型</span><span class="sxs-lookup"><span data-stu-id="51399-119">Type</span></span>|<span data-ttu-id="51399-120">说明</span><span class="sxs-lookup"><span data-stu-id="51399-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51399-121">displayName</span><span class="sxs-lookup"><span data-stu-id="51399-121">displayName</span></span>|<span data-ttu-id="51399-122">String</span><span class="sxs-lookup"><span data-stu-id="51399-122">String</span></span>|<span data-ttu-id="51399-123">状态报告的友好名称。</span><span class="sxs-lookup"><span data-stu-id="51399-123">Friendly name of the status report.</span></span> <span data-ttu-id="51399-124">继承自 [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="51399-124">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="51399-125">id</span><span class="sxs-lookup"><span data-stu-id="51399-125">id</span></span>|<span data-ttu-id="51399-126">String</span><span class="sxs-lookup"><span data-stu-id="51399-126">String</span></span>|<span data-ttu-id="51399-127">实体的键。</span><span class="sxs-lookup"><span data-stu-id="51399-127">Key of the entity.</span></span> <span data-ttu-id="51399-128">继承自 [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="51399-128">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="51399-129">version</span><span class="sxs-lookup"><span data-stu-id="51399-129">version</span></span>|<span data-ttu-id="51399-130">String</span><span class="sxs-lookup"><span data-stu-id="51399-130">String</span></span>|<span data-ttu-id="51399-131">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="51399-131">Version of the entity.</span></span> <span data-ttu-id="51399-132">继承自 [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="51399-132">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="51399-133">content</span><span class="sxs-lookup"><span data-stu-id="51399-133">content</span></span>|[<span data-ttu-id="51399-134">Json</span><span class="sxs-lookup"><span data-stu-id="51399-134">Json</span></span>](../resources/intune-mam-json.md)|<span data-ttu-id="51399-135">状态报告内容。</span><span class="sxs-lookup"><span data-stu-id="51399-135">Status report content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="51399-136">关系</span><span class="sxs-lookup"><span data-stu-id="51399-136">Relationships</span></span>
<span data-ttu-id="51399-137">无</span><span class="sxs-lookup"><span data-stu-id="51399-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="51399-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="51399-138">JSON Representation</span></span>
<span data-ttu-id="51399-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="51399-139">Here is a JSON representation of the resource.</span></span>
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




