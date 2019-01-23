---
title: managedAppStatus 资源类型
description: 表示组织的应用保护和配置状态。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7625543106b1ccf019df9622c1b0f37d40232f0c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415563"
---
# <a name="managedappstatus-resource-type"></a><span data-ttu-id="8b837-103">managedAppStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="8b837-103">managedAppStatus resource type</span></span>

> <span data-ttu-id="8b837-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="8b837-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="8b837-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="8b837-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8b837-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8b837-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8b837-107">表示组织的应用保护和配置状态。</span><span class="sxs-lookup"><span data-stu-id="8b837-107">Represents app protection and configuration status for the organization.</span></span>

## <a name="methods"></a><span data-ttu-id="8b837-108">方法</span><span class="sxs-lookup"><span data-stu-id="8b837-108">Methods</span></span>
|<span data-ttu-id="8b837-109">方法</span><span class="sxs-lookup"><span data-stu-id="8b837-109">Method</span></span>|<span data-ttu-id="8b837-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="8b837-110">Return Type</span></span>|<span data-ttu-id="8b837-111">说明</span><span class="sxs-lookup"><span data-stu-id="8b837-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8b837-112">列出 managedAppStatuses</span><span class="sxs-lookup"><span data-stu-id="8b837-112">List managedAppStatuses</span></span>](../api/intune-mam-managedappstatus-list.md)|<span data-ttu-id="8b837-113">[managedAppStatus](../resources/intune-mam-managedappstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8b837-113">[managedAppStatus](../resources/intune-mam-managedappstatus.md) collection</span></span>|<span data-ttu-id="8b837-114">列出 [managedAppStatus](../resources/intune-mam-managedappstatus.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8b837-114">List properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) objects.</span></span>|
|[<span data-ttu-id="8b837-115">获取 managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="8b837-115">Get managedAppStatus</span></span>](../api/intune-mam-managedappstatus-get.md)|[<span data-ttu-id="8b837-116">managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="8b837-116">managedAppStatus</span></span>](../resources/intune-mam-managedappstatus.md)|<span data-ttu-id="8b837-117">读取 [managedAppStatus](../resources/intune-mam-managedappstatus.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8b837-117">Read properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="8b837-118">属性</span><span class="sxs-lookup"><span data-stu-id="8b837-118">Properties</span></span>
|<span data-ttu-id="8b837-119">属性</span><span class="sxs-lookup"><span data-stu-id="8b837-119">Property</span></span>|<span data-ttu-id="8b837-120">类型</span><span class="sxs-lookup"><span data-stu-id="8b837-120">Type</span></span>|<span data-ttu-id="8b837-121">说明</span><span class="sxs-lookup"><span data-stu-id="8b837-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8b837-122">displayName</span><span class="sxs-lookup"><span data-stu-id="8b837-122">displayName</span></span>|<span data-ttu-id="8b837-123">String</span><span class="sxs-lookup"><span data-stu-id="8b837-123">String</span></span>|<span data-ttu-id="8b837-124">状态报告的友好名称。</span><span class="sxs-lookup"><span data-stu-id="8b837-124">Friendly name of the status report.</span></span>|
|<span data-ttu-id="8b837-125">id</span><span class="sxs-lookup"><span data-stu-id="8b837-125">id</span></span>|<span data-ttu-id="8b837-126">String</span><span class="sxs-lookup"><span data-stu-id="8b837-126">String</span></span>|<span data-ttu-id="8b837-127">实体的键。</span><span class="sxs-lookup"><span data-stu-id="8b837-127">Key of the entity.</span></span>|
|<span data-ttu-id="8b837-128">version</span><span class="sxs-lookup"><span data-stu-id="8b837-128">version</span></span>|<span data-ttu-id="8b837-129">String</span><span class="sxs-lookup"><span data-stu-id="8b837-129">String</span></span>|<span data-ttu-id="8b837-130">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="8b837-130">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8b837-131">关系</span><span class="sxs-lookup"><span data-stu-id="8b837-131">Relationships</span></span>
<span data-ttu-id="8b837-132">无</span><span class="sxs-lookup"><span data-stu-id="8b837-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8b837-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8b837-133">JSON Representation</span></span>
<span data-ttu-id="8b837-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8b837-134">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppStatus",
  "displayName": "String",
  "id": "String (identifier)",
  "version": "String"
}
```




