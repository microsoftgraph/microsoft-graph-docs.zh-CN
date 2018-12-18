---
title: managedAppStatusRaw 资源类型
description: 表示有关组织应用保护和配置的非类型化状态报告。
author: tfitzmac
ms.openlocfilehash: b4cb19b3fd9568afa65b50fea4fb4b3f0c8f1cc4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27322692"
---
# <a name="managedappstatusraw-resource-type"></a><span data-ttu-id="30911-103">managedAppStatusRaw 资源类型</span><span class="sxs-lookup"><span data-stu-id="30911-103">managedAppStatusRaw resource type</span></span>

> <span data-ttu-id="30911-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="30911-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="30911-105">表示有关组织应用保护和配置的非类型化状态报告。</span><span class="sxs-lookup"><span data-stu-id="30911-105">Represents an un-typed status report about organizations app protection and configuration.</span></span>

<span data-ttu-id="30911-106">继承自 [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="30911-106">Inherits from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>

## <a name="methods"></a><span data-ttu-id="30911-107">方法</span><span class="sxs-lookup"><span data-stu-id="30911-107">Methods</span></span>
|<span data-ttu-id="30911-108">方法</span><span class="sxs-lookup"><span data-stu-id="30911-108">Method</span></span>|<span data-ttu-id="30911-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="30911-109">Return Type</span></span>|<span data-ttu-id="30911-110">说明</span><span class="sxs-lookup"><span data-stu-id="30911-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="30911-111">列出 managedAppStatusRaws</span><span class="sxs-lookup"><span data-stu-id="30911-111">List managedAppStatusRaws</span></span>](../api/intune-mam-managedappstatusraw-list.md)|<span data-ttu-id="30911-112">[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) 集合</span><span class="sxs-lookup"><span data-stu-id="30911-112">[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) collection</span></span>|<span data-ttu-id="30911-113">列出 [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="30911-113">List properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) objects.</span></span>|
|[<span data-ttu-id="30911-114">获取 managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="30911-114">Get managedAppStatusRaw</span></span>](../api/intune-mam-managedappstatusraw-get.md)|[<span data-ttu-id="30911-115">managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="30911-115">managedAppStatusRaw</span></span>](../resources/intune-mam-managedappstatusraw.md)|<span data-ttu-id="30911-116">读取 [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="30911-116">Read properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="30911-117">属性</span><span class="sxs-lookup"><span data-stu-id="30911-117">Properties</span></span>
|<span data-ttu-id="30911-118">属性</span><span class="sxs-lookup"><span data-stu-id="30911-118">Property</span></span>|<span data-ttu-id="30911-119">类型</span><span class="sxs-lookup"><span data-stu-id="30911-119">Type</span></span>|<span data-ttu-id="30911-120">说明</span><span class="sxs-lookup"><span data-stu-id="30911-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="30911-121">displayName</span><span class="sxs-lookup"><span data-stu-id="30911-121">displayName</span></span>|<span data-ttu-id="30911-122">String</span><span class="sxs-lookup"><span data-stu-id="30911-122">String</span></span>|<span data-ttu-id="30911-123">状态报告的友好名称。</span><span class="sxs-lookup"><span data-stu-id="30911-123">Friendly name of the status report.</span></span> <span data-ttu-id="30911-124">继承自 [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="30911-124">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="30911-125">id</span><span class="sxs-lookup"><span data-stu-id="30911-125">id</span></span>|<span data-ttu-id="30911-126">String</span><span class="sxs-lookup"><span data-stu-id="30911-126">String</span></span>|<span data-ttu-id="30911-127">实体的键。</span><span class="sxs-lookup"><span data-stu-id="30911-127">Key of the entity.</span></span> <span data-ttu-id="30911-128">继承自 [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="30911-128">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="30911-129">version</span><span class="sxs-lookup"><span data-stu-id="30911-129">version</span></span>|<span data-ttu-id="30911-130">String</span><span class="sxs-lookup"><span data-stu-id="30911-130">String</span></span>|<span data-ttu-id="30911-131">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="30911-131">Version of the entity.</span></span> <span data-ttu-id="30911-132">继承自 [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="30911-132">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="30911-133">content</span><span class="sxs-lookup"><span data-stu-id="30911-133">content</span></span>|[<span data-ttu-id="30911-134">Json</span><span class="sxs-lookup"><span data-stu-id="30911-134">Json</span></span>](../resources/intune-mam-json.md)|<span data-ttu-id="30911-135">状态报告内容。</span><span class="sxs-lookup"><span data-stu-id="30911-135">Status report content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="30911-136">关系</span><span class="sxs-lookup"><span data-stu-id="30911-136">Relationships</span></span>
<span data-ttu-id="30911-137">无</span><span class="sxs-lookup"><span data-stu-id="30911-137">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="30911-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="30911-138">JSON Representation</span></span>
<span data-ttu-id="30911-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="30911-139">Here is a JSON representation of the resource.</span></span>
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



