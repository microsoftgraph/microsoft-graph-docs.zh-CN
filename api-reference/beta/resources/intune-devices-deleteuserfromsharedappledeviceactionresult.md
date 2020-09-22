---
title: deleteUserFromSharedAppleDeviceActionResult 资源类型
description: 从共享 Apple 设备删除用户操作结果
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6d615aa333f184569ec3f1424a4aa154407c1ce8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48060599"
---
# <a name="deleteuserfromsharedappledeviceactionresult-resource-type"></a><span data-ttu-id="c7cc9-103">deleteUserFromSharedAppleDeviceActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="c7cc9-103">deleteUserFromSharedAppleDeviceActionResult resource type</span></span>

<span data-ttu-id="c7cc9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c7cc9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c7cc9-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c7cc9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c7cc9-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c7cc9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c7cc9-107">从共享 Apple 设备删除用户操作结果</span><span class="sxs-lookup"><span data-stu-id="c7cc9-107">Delete user from shared apple device action result</span></span>


<span data-ttu-id="c7cc9-108">继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="c7cc9-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c7cc9-109">属性</span><span class="sxs-lookup"><span data-stu-id="c7cc9-109">Properties</span></span>
|<span data-ttu-id="c7cc9-110">属性</span><span class="sxs-lookup"><span data-stu-id="c7cc9-110">Property</span></span>|<span data-ttu-id="c7cc9-111">类型</span><span class="sxs-lookup"><span data-stu-id="c7cc9-111">Type</span></span>|<span data-ttu-id="c7cc9-112">说明</span><span class="sxs-lookup"><span data-stu-id="c7cc9-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7cc9-113">actionName</span><span class="sxs-lookup"><span data-stu-id="c7cc9-113">actionName</span></span>|<span data-ttu-id="c7cc9-114">String</span><span class="sxs-lookup"><span data-stu-id="c7cc9-114">String</span></span>|<span data-ttu-id="c7cc9-115">操作名称 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="c7cc9-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="c7cc9-116">actionState</span><span class="sxs-lookup"><span data-stu-id="c7cc9-116">actionState</span></span>|[<span data-ttu-id="c7cc9-117">actionState</span><span class="sxs-lookup"><span data-stu-id="c7cc9-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="c7cc9-118">继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)的操作的状态。</span><span class="sxs-lookup"><span data-stu-id="c7cc9-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="c7cc9-119">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed` 或 `notSupported`。</span><span class="sxs-lookup"><span data-stu-id="c7cc9-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="c7cc9-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="c7cc9-120">startDateTime</span></span>|<span data-ttu-id="c7cc9-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c7cc9-121">DateTimeOffset</span></span>|<span data-ttu-id="c7cc9-122">操作启动的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="c7cc9-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="c7cc9-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="c7cc9-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="c7cc9-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c7cc9-124">DateTimeOffset</span></span>|<span data-ttu-id="c7cc9-125">操作状态上次更新的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="c7cc9-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="c7cc9-126">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c7cc9-126">userPrincipalName</span></span>|<span data-ttu-id="c7cc9-127">String</span><span class="sxs-lookup"><span data-stu-id="c7cc9-127">String</span></span>|<span data-ttu-id="c7cc9-128">要删除的用户的用户主体名称</span><span class="sxs-lookup"><span data-stu-id="c7cc9-128">User principal name of the user to be deleted</span></span>|

## <a name="relationships"></a><span data-ttu-id="c7cc9-129">关系</span><span class="sxs-lookup"><span data-stu-id="c7cc9-129">Relationships</span></span>
<span data-ttu-id="c7cc9-130">无</span><span class="sxs-lookup"><span data-stu-id="c7cc9-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c7cc9-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c7cc9-131">JSON Representation</span></span>
<span data-ttu-id="c7cc9-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c7cc9-132">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deleteUserFromSharedAppleDeviceActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deleteUserFromSharedAppleDeviceActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "userPrincipalName": "String"
}
```






