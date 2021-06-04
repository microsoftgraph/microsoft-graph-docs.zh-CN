---
title: managedAppStatusRaw 资源类型
description: 表示有关组织应用保护和配置的非类型化状态报告。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1d29ec2d96d38c6bc1f2fccf5fb5b36e16e1c5be
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752768"
---
# <a name="managedappstatusraw-resource-type"></a><span data-ttu-id="b3c5a-103">managedAppStatusRaw 资源类型</span><span class="sxs-lookup"><span data-stu-id="b3c5a-103">managedAppStatusRaw resource type</span></span>

<span data-ttu-id="b3c5a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b3c5a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b3c5a-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b3c5a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b3c5a-106">表示有关组织应用保护和配置的非类型化状态报告。</span><span class="sxs-lookup"><span data-stu-id="b3c5a-106">Represents an un-typed status report about organizations app protection and configuration.</span></span>


<span data-ttu-id="b3c5a-107">继承自 [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="b3c5a-107">Inherits from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>

## <a name="methods"></a><span data-ttu-id="b3c5a-108">Methods</span><span class="sxs-lookup"><span data-stu-id="b3c5a-108">Methods</span></span>
|<span data-ttu-id="b3c5a-109">方法</span><span class="sxs-lookup"><span data-stu-id="b3c5a-109">Method</span></span>|<span data-ttu-id="b3c5a-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="b3c5a-110">Return Type</span></span>|<span data-ttu-id="b3c5a-111">Description</span><span class="sxs-lookup"><span data-stu-id="b3c5a-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b3c5a-112">列出 managedAppStatusRaws</span><span class="sxs-lookup"><span data-stu-id="b3c5a-112">List managedAppStatusRaws</span></span>](../api/intune-mam-managedappstatusraw-list.md)|<span data-ttu-id="b3c5a-113">[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b3c5a-113">[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) collection</span></span>|<span data-ttu-id="b3c5a-114">列出 [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b3c5a-114">List properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) objects.</span></span>|
|[<span data-ttu-id="b3c5a-115">获取 managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="b3c5a-115">Get managedAppStatusRaw</span></span>](../api/intune-mam-managedappstatusraw-get.md)|[<span data-ttu-id="b3c5a-116">managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="b3c5a-116">managedAppStatusRaw</span></span>](../resources/intune-mam-managedappstatusraw.md)|<span data-ttu-id="b3c5a-117">读取 [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b3c5a-117">Read properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b3c5a-118">属性</span><span class="sxs-lookup"><span data-stu-id="b3c5a-118">Properties</span></span>
|<span data-ttu-id="b3c5a-119">属性</span><span class="sxs-lookup"><span data-stu-id="b3c5a-119">Property</span></span>|<span data-ttu-id="b3c5a-120">类型</span><span class="sxs-lookup"><span data-stu-id="b3c5a-120">Type</span></span>|<span data-ttu-id="b3c5a-121">说明</span><span class="sxs-lookup"><span data-stu-id="b3c5a-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b3c5a-122">displayName</span><span class="sxs-lookup"><span data-stu-id="b3c5a-122">displayName</span></span>|<span data-ttu-id="b3c5a-123">String</span><span class="sxs-lookup"><span data-stu-id="b3c5a-123">String</span></span>|<span data-ttu-id="b3c5a-124">状态报告的友好名称。</span><span class="sxs-lookup"><span data-stu-id="b3c5a-124">Friendly name of the status report.</span></span> <span data-ttu-id="b3c5a-125">继承自 [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="b3c5a-125">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="b3c5a-126">id</span><span class="sxs-lookup"><span data-stu-id="b3c5a-126">id</span></span>|<span data-ttu-id="b3c5a-127">String</span><span class="sxs-lookup"><span data-stu-id="b3c5a-127">String</span></span>|<span data-ttu-id="b3c5a-128">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b3c5a-128">Key of the entity.</span></span> <span data-ttu-id="b3c5a-129">继承自 [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="b3c5a-129">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="b3c5a-130">version</span><span class="sxs-lookup"><span data-stu-id="b3c5a-130">version</span></span>|<span data-ttu-id="b3c5a-131">String</span><span class="sxs-lookup"><span data-stu-id="b3c5a-131">String</span></span>|<span data-ttu-id="b3c5a-132">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="b3c5a-132">Version of the entity.</span></span> <span data-ttu-id="b3c5a-133">继承自 [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="b3c5a-133">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="b3c5a-134">content</span><span class="sxs-lookup"><span data-stu-id="b3c5a-134">content</span></span>|[<span data-ttu-id="b3c5a-135">Json</span><span class="sxs-lookup"><span data-stu-id="b3c5a-135">Json</span></span>](../resources/intune-mam-json.md)|<span data-ttu-id="b3c5a-136">状态报告内容。</span><span class="sxs-lookup"><span data-stu-id="b3c5a-136">Status report content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b3c5a-137">关系</span><span class="sxs-lookup"><span data-stu-id="b3c5a-137">Relationships</span></span>
<span data-ttu-id="b3c5a-138">无</span><span class="sxs-lookup"><span data-stu-id="b3c5a-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b3c5a-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b3c5a-139">JSON Representation</span></span>
<span data-ttu-id="b3c5a-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b3c5a-140">Here is a JSON representation of the resource.</span></span>
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




