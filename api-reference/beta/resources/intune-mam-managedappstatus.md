---
title: managedAppStatus 资源类型
description: 表示组织的应用保护和配置状态。
ms.openlocfilehash: 659e89acb6741c7a3f7aad072bb658ce52e9e5cc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27047783"
---
# <a name="managedappstatus-resource-type"></a><span data-ttu-id="42c4a-103">managedAppStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="42c4a-103">managedAppStatus resource type</span></span>

> <span data-ttu-id="42c4a-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="42c4a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="42c4a-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="42c4a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="42c4a-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="42c4a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="42c4a-107">表示组织的应用保护和配置状态。</span><span class="sxs-lookup"><span data-stu-id="42c4a-107">Represents app protection and configuration status for the organization.</span></span>
## <a name="methods"></a><span data-ttu-id="42c4a-108">方法</span><span class="sxs-lookup"><span data-stu-id="42c4a-108">Methods</span></span>
|<span data-ttu-id="42c4a-109">方法</span><span class="sxs-lookup"><span data-stu-id="42c4a-109">Method</span></span>|<span data-ttu-id="42c4a-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="42c4a-110">Return Type</span></span>|<span data-ttu-id="42c4a-111">说明</span><span class="sxs-lookup"><span data-stu-id="42c4a-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="42c4a-112">列出 managedAppStatuses</span><span class="sxs-lookup"><span data-stu-id="42c4a-112">List managedAppStatuses</span></span>](../api/intune-mam-managedappstatus-list.md)|<span data-ttu-id="42c4a-113">[managedAppStatus](../resources/intune-mam-managedappstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="42c4a-113">[managedAppStatus](../resources/intune-mam-managedappstatus.md) collection</span></span>|<span data-ttu-id="42c4a-114">列出 [managedAppStatus](../resources/intune-mam-managedappstatus.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="42c4a-114">List properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) objects.</span></span>|
|[<span data-ttu-id="42c4a-115">获取 managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="42c4a-115">Get managedAppStatus</span></span>](../api/intune-mam-managedappstatus-get.md)|[<span data-ttu-id="42c4a-116">managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="42c4a-116">managedAppStatus</span></span>](../resources/intune-mam-managedappstatus.md)|<span data-ttu-id="42c4a-117">读取 [managedAppStatus](../resources/intune-mam-managedappstatus.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="42c4a-117">Read properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="42c4a-118">属性</span><span class="sxs-lookup"><span data-stu-id="42c4a-118">Properties</span></span>
|<span data-ttu-id="42c4a-119">属性</span><span class="sxs-lookup"><span data-stu-id="42c4a-119">Property</span></span>|<span data-ttu-id="42c4a-120">类型</span><span class="sxs-lookup"><span data-stu-id="42c4a-120">Type</span></span>|<span data-ttu-id="42c4a-121">说明</span><span class="sxs-lookup"><span data-stu-id="42c4a-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42c4a-122">displayName</span><span class="sxs-lookup"><span data-stu-id="42c4a-122">displayName</span></span>|<span data-ttu-id="42c4a-123">String</span><span class="sxs-lookup"><span data-stu-id="42c4a-123">String</span></span>|<span data-ttu-id="42c4a-124">状态报告的友好名称。</span><span class="sxs-lookup"><span data-stu-id="42c4a-124">Friendly name of the status report.</span></span>|
|<span data-ttu-id="42c4a-125">id</span><span class="sxs-lookup"><span data-stu-id="42c4a-125">id</span></span>|<span data-ttu-id="42c4a-126">String</span><span class="sxs-lookup"><span data-stu-id="42c4a-126">String</span></span>|<span data-ttu-id="42c4a-127">实体的键。</span><span class="sxs-lookup"><span data-stu-id="42c4a-127">Key of the entity.</span></span>|
|<span data-ttu-id="42c4a-128">version</span><span class="sxs-lookup"><span data-stu-id="42c4a-128">version</span></span>|<span data-ttu-id="42c4a-129">String</span><span class="sxs-lookup"><span data-stu-id="42c4a-129">String</span></span>|<span data-ttu-id="42c4a-130">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="42c4a-130">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="42c4a-131">关系</span><span class="sxs-lookup"><span data-stu-id="42c4a-131">Relationships</span></span>
<span data-ttu-id="42c4a-132">无</span><span class="sxs-lookup"><span data-stu-id="42c4a-132">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="42c4a-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="42c4a-133">JSON Representation</span></span>
<span data-ttu-id="42c4a-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="42c4a-134">Here is a JSON representation of the resource.</span></span>
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





