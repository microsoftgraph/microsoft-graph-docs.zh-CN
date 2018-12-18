---
title: managedAppStatusRaw 资源类型
description: 表示有关组织应用保护和配置的非类型化状态报告。
author: tfitzmac
ms.openlocfilehash: 9b7c957451e3fc92ad79ef10433e26bf39fd1c48
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27331925"
---
# <a name="managedappstatusraw-resource-type"></a><span data-ttu-id="0f3d3-103">managedAppStatusRaw 资源类型</span><span class="sxs-lookup"><span data-stu-id="0f3d3-103">managedAppStatusRaw resource type</span></span>

> <span data-ttu-id="0f3d3-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="0f3d3-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0f3d3-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="0f3d3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0f3d3-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="0f3d3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0f3d3-107">表示有关组织应用保护和配置的非类型化状态报告。</span><span class="sxs-lookup"><span data-stu-id="0f3d3-107">Represents an un-typed status report about organizations app protection and configuration.</span></span>

<span data-ttu-id="0f3d3-108">继承自 [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="0f3d3-108">Inherits from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>

## <a name="methods"></a><span data-ttu-id="0f3d3-109">方法</span><span class="sxs-lookup"><span data-stu-id="0f3d3-109">Methods</span></span>
|<span data-ttu-id="0f3d3-110">方法</span><span class="sxs-lookup"><span data-stu-id="0f3d3-110">Method</span></span>|<span data-ttu-id="0f3d3-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="0f3d3-111">Return Type</span></span>|<span data-ttu-id="0f3d3-112">说明</span><span class="sxs-lookup"><span data-stu-id="0f3d3-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0f3d3-113">列出 managedAppStatusRaws</span><span class="sxs-lookup"><span data-stu-id="0f3d3-113">List managedAppStatusRaws</span></span>](../api/intune-mam-managedappstatusraw-list.md)|<span data-ttu-id="0f3d3-114">[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0f3d3-114">[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) collection</span></span>|<span data-ttu-id="0f3d3-115">列出 [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0f3d3-115">List properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) objects.</span></span>|
|[<span data-ttu-id="0f3d3-116">获取 managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="0f3d3-116">Get managedAppStatusRaw</span></span>](../api/intune-mam-managedappstatusraw-get.md)|[<span data-ttu-id="0f3d3-117">managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="0f3d3-117">managedAppStatusRaw</span></span>](../resources/intune-mam-managedappstatusraw.md)|<span data-ttu-id="0f3d3-118">读取 [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0f3d3-118">Read properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0f3d3-119">属性</span><span class="sxs-lookup"><span data-stu-id="0f3d3-119">Properties</span></span>
|<span data-ttu-id="0f3d3-120">属性</span><span class="sxs-lookup"><span data-stu-id="0f3d3-120">Property</span></span>|<span data-ttu-id="0f3d3-121">类型</span><span class="sxs-lookup"><span data-stu-id="0f3d3-121">Type</span></span>|<span data-ttu-id="0f3d3-122">说明</span><span class="sxs-lookup"><span data-stu-id="0f3d3-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f3d3-123">displayName</span><span class="sxs-lookup"><span data-stu-id="0f3d3-123">displayName</span></span>|<span data-ttu-id="0f3d3-124">String</span><span class="sxs-lookup"><span data-stu-id="0f3d3-124">String</span></span>|<span data-ttu-id="0f3d3-125">状态报告的友好名称。</span><span class="sxs-lookup"><span data-stu-id="0f3d3-125">Friendly name of the status report.</span></span> <span data-ttu-id="0f3d3-126">继承自 [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="0f3d3-126">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="0f3d3-127">id</span><span class="sxs-lookup"><span data-stu-id="0f3d3-127">id</span></span>|<span data-ttu-id="0f3d3-128">String</span><span class="sxs-lookup"><span data-stu-id="0f3d3-128">String</span></span>|<span data-ttu-id="0f3d3-129">实体的键。</span><span class="sxs-lookup"><span data-stu-id="0f3d3-129">Key of the entity.</span></span> <span data-ttu-id="0f3d3-130">继承自 [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="0f3d3-130">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="0f3d3-131">version</span><span class="sxs-lookup"><span data-stu-id="0f3d3-131">version</span></span>|<span data-ttu-id="0f3d3-132">String</span><span class="sxs-lookup"><span data-stu-id="0f3d3-132">String</span></span>|<span data-ttu-id="0f3d3-133">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="0f3d3-133">Version of the entity.</span></span> <span data-ttu-id="0f3d3-134">继承自 [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="0f3d3-134">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="0f3d3-135">content</span><span class="sxs-lookup"><span data-stu-id="0f3d3-135">content</span></span>|[<span data-ttu-id="0f3d3-136">Json</span><span class="sxs-lookup"><span data-stu-id="0f3d3-136">Json</span></span>](../resources/intune-mam-json.md)|<span data-ttu-id="0f3d3-137">状态报告内容。</span><span class="sxs-lookup"><span data-stu-id="0f3d3-137">Status report content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0f3d3-138">关系</span><span class="sxs-lookup"><span data-stu-id="0f3d3-138">Relationships</span></span>
<span data-ttu-id="0f3d3-139">无</span><span class="sxs-lookup"><span data-stu-id="0f3d3-139">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0f3d3-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0f3d3-140">JSON Representation</span></span>
<span data-ttu-id="0f3d3-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0f3d3-141">Here is a JSON representation of the resource.</span></span>
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





