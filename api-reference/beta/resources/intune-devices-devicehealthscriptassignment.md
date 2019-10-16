---
title: deviceHealthScriptAssignment 资源类型
description: 包含用于将设备管理脚本分配给组的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a37d36fd5b36384d62ef656b9d36a7ed870e3586
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37539090"
---
# <a name="devicehealthscriptassignment-resource-type"></a><span data-ttu-id="177d6-103">deviceHealthScriptAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="177d6-103">deviceHealthScriptAssignment resource type</span></span>

> <span data-ttu-id="177d6-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="177d6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="177d6-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="177d6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="177d6-106">包含用于将设备管理脚本分配给组的属性。</span><span class="sxs-lookup"><span data-stu-id="177d6-106">Contains properties used to assign a device management script to a group.</span></span>

## <a name="methods"></a><span data-ttu-id="177d6-107">方法</span><span class="sxs-lookup"><span data-stu-id="177d6-107">Methods</span></span>
|<span data-ttu-id="177d6-108">方法</span><span class="sxs-lookup"><span data-stu-id="177d6-108">Method</span></span>|<span data-ttu-id="177d6-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="177d6-109">Return Type</span></span>|<span data-ttu-id="177d6-110">说明</span><span class="sxs-lookup"><span data-stu-id="177d6-110">Description</span></span>|
|:---|:---|:---|
<span data-ttu-id="177d6-111">无</span><span class="sxs-lookup"><span data-stu-id="177d6-111">None</span></span>

## <a name="properties"></a><span data-ttu-id="177d6-112">属性</span><span class="sxs-lookup"><span data-stu-id="177d6-112">Properties</span></span>
|<span data-ttu-id="177d6-113">属性</span><span class="sxs-lookup"><span data-stu-id="177d6-113">Property</span></span>|<span data-ttu-id="177d6-114">类型</span><span class="sxs-lookup"><span data-stu-id="177d6-114">Type</span></span>|<span data-ttu-id="177d6-115">说明</span><span class="sxs-lookup"><span data-stu-id="177d6-115">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="177d6-116">id</span><span class="sxs-lookup"><span data-stu-id="177d6-116">id</span></span>|<span data-ttu-id="177d6-117">字符串</span><span class="sxs-lookup"><span data-stu-id="177d6-117">String</span></span>|<span data-ttu-id="177d6-118">设备运行状况脚本分配实体的键</span><span class="sxs-lookup"><span data-stu-id="177d6-118">Key of the device health script assignment entity</span></span>|
|<span data-ttu-id="177d6-119">target</span><span class="sxs-lookup"><span data-stu-id="177d6-119">target</span></span>|[<span data-ttu-id="177d6-120">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="177d6-120">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="177d6-121">将脚本设定为的 Azure Active Directory 组</span><span class="sxs-lookup"><span data-stu-id="177d6-121">The Azure Active Directory group we are targeting the script to</span></span>|
|<span data-ttu-id="177d6-122">runRemediationScript</span><span class="sxs-lookup"><span data-stu-id="177d6-122">runRemediationScript</span></span>|<span data-ttu-id="177d6-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="177d6-123">Boolean</span></span>|<span data-ttu-id="177d6-124">确定是只运行检测脚本还是运行两个检测脚本和修正脚本</span><span class="sxs-lookup"><span data-stu-id="177d6-124">Determine whether we want to run detection script only or run both detection script and remediation script</span></span>|
|<span data-ttu-id="177d6-125">runSchedule</span><span class="sxs-lookup"><span data-stu-id="177d6-125">runSchedule</span></span>|[<span data-ttu-id="177d6-126">runSchedule</span><span class="sxs-lookup"><span data-stu-id="177d6-126">runSchedule</span></span>](../resources/intune-devices-runschedule.md)|<span data-ttu-id="177d6-127">将脚本设定为的 Azure Active Directory 组</span><span class="sxs-lookup"><span data-stu-id="177d6-127">The Azure Active Directory group we are targeting the script to</span></span>|

## <a name="relationships"></a><span data-ttu-id="177d6-128">关系</span><span class="sxs-lookup"><span data-stu-id="177d6-128">Relationships</span></span>
<span data-ttu-id="177d6-129">无</span><span class="sxs-lookup"><span data-stu-id="177d6-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="177d6-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="177d6-130">JSON Representation</span></span>
<span data-ttu-id="177d6-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="177d6-131">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceHealthScriptAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "runRemediationScript": true,
  "runSchedule": {
      "@odata.type": "microsoft.graph.runSchedule"
  }
}
```



