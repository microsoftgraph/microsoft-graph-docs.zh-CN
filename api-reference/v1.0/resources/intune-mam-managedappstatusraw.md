---
title: managedAppStatusRaw 资源类型
description: 表示有关组织应用保护和配置的非类型化状态报告。
ms.openlocfilehash: 9576123e39be2ae37052926342fb634c21086371
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27010716"
---
# <a name="managedappstatusraw-resource-type"></a><span data-ttu-id="59b13-103">managedAppStatusRaw 资源类型</span><span class="sxs-lookup"><span data-stu-id="59b13-103">managedAppStatusRaw resource type</span></span>

> <span data-ttu-id="59b13-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="59b13-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="59b13-105">表示有关组织应用保护和配置的非类型化状态报告。</span><span class="sxs-lookup"><span data-stu-id="59b13-105">Represents an un-typed status report about organizations app protection and configuration.</span></span>

<span data-ttu-id="59b13-106">继承自 [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="59b13-106">Inherits from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>

## <a name="methods"></a><span data-ttu-id="59b13-107">方法</span><span class="sxs-lookup"><span data-stu-id="59b13-107">Methods</span></span>
|<span data-ttu-id="59b13-108">方法</span><span class="sxs-lookup"><span data-stu-id="59b13-108">Method</span></span>|<span data-ttu-id="59b13-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="59b13-109">Return Type</span></span>|<span data-ttu-id="59b13-110">说明</span><span class="sxs-lookup"><span data-stu-id="59b13-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="59b13-111">列出 managedAppStatusRaws</span><span class="sxs-lookup"><span data-stu-id="59b13-111">List managedAppStatusRaws</span></span>](../api/intune-mam-managedappstatusraw-list.md)|<span data-ttu-id="59b13-112">[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) 集合</span><span class="sxs-lookup"><span data-stu-id="59b13-112">[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) collection</span></span>|<span data-ttu-id="59b13-113">列出 [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="59b13-113">List properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) objects.</span></span>|
|[<span data-ttu-id="59b13-114">获取 managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="59b13-114">Get managedAppStatusRaw</span></span>](../api/intune-mam-managedappstatusraw-get.md)|[<span data-ttu-id="59b13-115">managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="59b13-115">managedAppStatusRaw</span></span>](../resources/intune-mam-managedappstatusraw.md)|<span data-ttu-id="59b13-116">读取 [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="59b13-116">Read properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="59b13-117">属性</span><span class="sxs-lookup"><span data-stu-id="59b13-117">Properties</span></span>
|<span data-ttu-id="59b13-118">属性</span><span class="sxs-lookup"><span data-stu-id="59b13-118">Property</span></span>|<span data-ttu-id="59b13-119">类型</span><span class="sxs-lookup"><span data-stu-id="59b13-119">Type</span></span>|<span data-ttu-id="59b13-120">说明</span><span class="sxs-lookup"><span data-stu-id="59b13-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="59b13-121">displayName</span><span class="sxs-lookup"><span data-stu-id="59b13-121">displayName</span></span>|<span data-ttu-id="59b13-122">String</span><span class="sxs-lookup"><span data-stu-id="59b13-122">String</span></span>|<span data-ttu-id="59b13-123">状态报告的友好名称。</span><span class="sxs-lookup"><span data-stu-id="59b13-123">Friendly name of the status report.</span></span> <span data-ttu-id="59b13-124">继承自 [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="59b13-124">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="59b13-125">id</span><span class="sxs-lookup"><span data-stu-id="59b13-125">id</span></span>|<span data-ttu-id="59b13-126">String</span><span class="sxs-lookup"><span data-stu-id="59b13-126">String</span></span>|<span data-ttu-id="59b13-127">实体的键。</span><span class="sxs-lookup"><span data-stu-id="59b13-127">Key of the entity.</span></span> <span data-ttu-id="59b13-128">继承自 [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="59b13-128">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="59b13-129">version</span><span class="sxs-lookup"><span data-stu-id="59b13-129">version</span></span>|<span data-ttu-id="59b13-130">String</span><span class="sxs-lookup"><span data-stu-id="59b13-130">String</span></span>|<span data-ttu-id="59b13-131">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="59b13-131">Version of the entity.</span></span> <span data-ttu-id="59b13-132">继承自 [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="59b13-132">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="59b13-133">content</span><span class="sxs-lookup"><span data-stu-id="59b13-133">content</span></span>|[<span data-ttu-id="59b13-134">Json</span><span class="sxs-lookup"><span data-stu-id="59b13-134">Json</span></span>](../resources/intune-mam-json.md)|<span data-ttu-id="59b13-135">状态报告内容。</span><span class="sxs-lookup"><span data-stu-id="59b13-135">Status report content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="59b13-136">关系</span><span class="sxs-lookup"><span data-stu-id="59b13-136">Relationships</span></span>
<span data-ttu-id="59b13-137">无</span><span class="sxs-lookup"><span data-stu-id="59b13-137">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="59b13-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="59b13-138">JSON Representation</span></span>
<span data-ttu-id="59b13-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="59b13-139">Here is a JSON representation of the resource.</span></span>
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



