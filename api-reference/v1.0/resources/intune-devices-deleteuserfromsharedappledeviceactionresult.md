---
title: deleteUserFromSharedAppleDeviceActionResult 资源类型
description: 从共享 Apple 设备删除用户操作结果
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 5dffabe173e1e0bd69cd1fab2da767131c3d246d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36027480"
---
# <a name="deleteuserfromsharedappledeviceactionresult-resource-type"></a><span data-ttu-id="9a460-103">deleteUserFromSharedAppleDeviceActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="9a460-103">deleteUserFromSharedAppleDeviceActionResult resource type</span></span>

> <span data-ttu-id="9a460-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9a460-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9a460-105">从共享 Apple 设备删除用户操作结果</span><span class="sxs-lookup"><span data-stu-id="9a460-105">Delete user from shared apple device action result</span></span>


<span data-ttu-id="9a460-106">继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="9a460-106">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="9a460-107">属性</span><span class="sxs-lookup"><span data-stu-id="9a460-107">Properties</span></span>
|<span data-ttu-id="9a460-108">属性</span><span class="sxs-lookup"><span data-stu-id="9a460-108">Property</span></span>|<span data-ttu-id="9a460-109">类型</span><span class="sxs-lookup"><span data-stu-id="9a460-109">Type</span></span>|<span data-ttu-id="9a460-110">说明</span><span class="sxs-lookup"><span data-stu-id="9a460-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9a460-111">actionName</span><span class="sxs-lookup"><span data-stu-id="9a460-111">actionName</span></span>|<span data-ttu-id="9a460-112">String</span><span class="sxs-lookup"><span data-stu-id="9a460-112">String</span></span>|<span data-ttu-id="9a460-113">操作名称 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="9a460-113">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="9a460-114">actionState</span><span class="sxs-lookup"><span data-stu-id="9a460-114">actionState</span></span>|[<span data-ttu-id="9a460-115">actionState</span><span class="sxs-lookup"><span data-stu-id="9a460-115">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="9a460-116">继承自[deviceActionResult](../resources/intune-devices-deviceactionresult.md)的操作的状态。</span><span class="sxs-lookup"><span data-stu-id="9a460-116">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="9a460-117">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed` 或 `notSupported`。</span><span class="sxs-lookup"><span data-stu-id="9a460-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="9a460-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="9a460-118">startDateTime</span></span>|<span data-ttu-id="9a460-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9a460-119">DateTimeOffset</span></span>|<span data-ttu-id="9a460-120">操作启动的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="9a460-120">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="9a460-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="9a460-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="9a460-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9a460-122">DateTimeOffset</span></span>|<span data-ttu-id="9a460-123">操作状态上次更新的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="9a460-123">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="9a460-124">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="9a460-124">userPrincipalName</span></span>|<span data-ttu-id="9a460-125">String</span><span class="sxs-lookup"><span data-stu-id="9a460-125">String</span></span>|<span data-ttu-id="9a460-126">要删除的用户的用户主体名称</span><span class="sxs-lookup"><span data-stu-id="9a460-126">User principal name of the user to be deleted</span></span>|

## <a name="relationships"></a><span data-ttu-id="9a460-127">关系</span><span class="sxs-lookup"><span data-stu-id="9a460-127">Relationships</span></span>
<span data-ttu-id="9a460-128">无</span><span class="sxs-lookup"><span data-stu-id="9a460-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9a460-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9a460-129">JSON Representation</span></span>
<span data-ttu-id="9a460-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9a460-130">Here is a JSON representation of the resource.</span></span>
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



