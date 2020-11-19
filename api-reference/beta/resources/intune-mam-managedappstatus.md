---
title: managedAppStatus 资源类型
description: 表示组织的应用保护和配置状态。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e3a43214f2c9157de1ebf690eb9d43504e5224d7
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49266786"
---
# <a name="managedappstatus-resource-type"></a><span data-ttu-id="c7297-103">managedAppStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="c7297-103">managedAppStatus resource type</span></span>

<span data-ttu-id="c7297-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c7297-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c7297-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c7297-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c7297-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c7297-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c7297-107">表示组织的应用保护和配置状态。</span><span class="sxs-lookup"><span data-stu-id="c7297-107">Represents app protection and configuration status for the organization.</span></span>

## <a name="methods"></a><span data-ttu-id="c7297-108">方法</span><span class="sxs-lookup"><span data-stu-id="c7297-108">Methods</span></span>
|<span data-ttu-id="c7297-109">方法</span><span class="sxs-lookup"><span data-stu-id="c7297-109">Method</span></span>|<span data-ttu-id="c7297-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="c7297-110">Return Type</span></span>|<span data-ttu-id="c7297-111">说明</span><span class="sxs-lookup"><span data-stu-id="c7297-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c7297-112">列出 managedAppStatuses</span><span class="sxs-lookup"><span data-stu-id="c7297-112">List managedAppStatuses</span></span>](../api/intune-mam-managedappstatus-list.md)|<span data-ttu-id="c7297-113">[managedAppStatus](../resources/intune-mam-managedappstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c7297-113">[managedAppStatus](../resources/intune-mam-managedappstatus.md) collection</span></span>|<span data-ttu-id="c7297-114">列出 [managedAppStatus](../resources/intune-mam-managedappstatus.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c7297-114">List properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) objects.</span></span>|
|[<span data-ttu-id="c7297-115">获取 managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="c7297-115">Get managedAppStatus</span></span>](../api/intune-mam-managedappstatus-get.md)|[<span data-ttu-id="c7297-116">managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="c7297-116">managedAppStatus</span></span>](../resources/intune-mam-managedappstatus.md)|<span data-ttu-id="c7297-117">读取 [managedAppStatus](../resources/intune-mam-managedappstatus.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c7297-117">Read properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c7297-118">属性</span><span class="sxs-lookup"><span data-stu-id="c7297-118">Properties</span></span>
|<span data-ttu-id="c7297-119">属性</span><span class="sxs-lookup"><span data-stu-id="c7297-119">Property</span></span>|<span data-ttu-id="c7297-120">类型</span><span class="sxs-lookup"><span data-stu-id="c7297-120">Type</span></span>|<span data-ttu-id="c7297-121">说明</span><span class="sxs-lookup"><span data-stu-id="c7297-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7297-122">displayName</span><span class="sxs-lookup"><span data-stu-id="c7297-122">displayName</span></span>|<span data-ttu-id="c7297-123">字符串</span><span class="sxs-lookup"><span data-stu-id="c7297-123">String</span></span>|<span data-ttu-id="c7297-124">状态报告的友好名称。</span><span class="sxs-lookup"><span data-stu-id="c7297-124">Friendly name of the status report.</span></span>|
|<span data-ttu-id="c7297-125">id</span><span class="sxs-lookup"><span data-stu-id="c7297-125">id</span></span>|<span data-ttu-id="c7297-126">字符串</span><span class="sxs-lookup"><span data-stu-id="c7297-126">String</span></span>|<span data-ttu-id="c7297-127">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c7297-127">Key of the entity.</span></span>|
|<span data-ttu-id="c7297-128">version</span><span class="sxs-lookup"><span data-stu-id="c7297-128">version</span></span>|<span data-ttu-id="c7297-129">String</span><span class="sxs-lookup"><span data-stu-id="c7297-129">String</span></span>|<span data-ttu-id="c7297-130">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="c7297-130">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c7297-131">关系</span><span class="sxs-lookup"><span data-stu-id="c7297-131">Relationships</span></span>
<span data-ttu-id="c7297-132">无</span><span class="sxs-lookup"><span data-stu-id="c7297-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c7297-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c7297-133">JSON Representation</span></span>
<span data-ttu-id="c7297-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c7297-134">Here is a JSON representation of the resource.</span></span>
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




