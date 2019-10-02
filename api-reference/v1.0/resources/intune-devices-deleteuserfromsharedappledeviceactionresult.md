---
title: deleteUserFromSharedAppleDeviceActionResult 资源类型
description: 从共享 Apple 设备删除用户操作结果
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 88ed9a813b678381b32f2b054933e9d3ad28683d
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37357029"
---
# <a name="deleteuserfromsharedappledeviceactionresult-resource-type"></a><span data-ttu-id="4ef7c-103">deleteUserFromSharedAppleDeviceActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="4ef7c-103">deleteUserFromSharedAppleDeviceActionResult resource type</span></span>

> <span data-ttu-id="4ef7c-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4ef7c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4ef7c-105">从共享 Apple 设备删除用户操作结果</span><span class="sxs-lookup"><span data-stu-id="4ef7c-105">Delete user from shared apple device action result</span></span>


<span data-ttu-id="4ef7c-106">继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="4ef7c-106">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4ef7c-107">属性</span><span class="sxs-lookup"><span data-stu-id="4ef7c-107">Properties</span></span>
|<span data-ttu-id="4ef7c-108">属性</span><span class="sxs-lookup"><span data-stu-id="4ef7c-108">Property</span></span>|<span data-ttu-id="4ef7c-109">类型</span><span class="sxs-lookup"><span data-stu-id="4ef7c-109">Type</span></span>|<span data-ttu-id="4ef7c-110">说明</span><span class="sxs-lookup"><span data-stu-id="4ef7c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4ef7c-111">actionName</span><span class="sxs-lookup"><span data-stu-id="4ef7c-111">actionName</span></span>|<span data-ttu-id="4ef7c-112">String</span><span class="sxs-lookup"><span data-stu-id="4ef7c-112">String</span></span>|<span data-ttu-id="4ef7c-113">操作名称 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="4ef7c-113">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="4ef7c-114">actionState</span><span class="sxs-lookup"><span data-stu-id="4ef7c-114">actionState</span></span>|[<span data-ttu-id="4ef7c-115">actionState</span><span class="sxs-lookup"><span data-stu-id="4ef7c-115">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="4ef7c-116">继承自[deviceActionResult](../resources/intune-devices-deviceactionresult.md)的操作的状态。</span><span class="sxs-lookup"><span data-stu-id="4ef7c-116">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="4ef7c-117">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed` 或 `notSupported`。</span><span class="sxs-lookup"><span data-stu-id="4ef7c-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="4ef7c-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="4ef7c-118">startDateTime</span></span>|<span data-ttu-id="4ef7c-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4ef7c-119">DateTimeOffset</span></span>|<span data-ttu-id="4ef7c-120">操作启动的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="4ef7c-120">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="4ef7c-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="4ef7c-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="4ef7c-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4ef7c-122">DateTimeOffset</span></span>|<span data-ttu-id="4ef7c-123">操作状态上次更新的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="4ef7c-123">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="4ef7c-124">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="4ef7c-124">userPrincipalName</span></span>|<span data-ttu-id="4ef7c-125">String</span><span class="sxs-lookup"><span data-stu-id="4ef7c-125">String</span></span>|<span data-ttu-id="4ef7c-126">要删除的用户的用户主体名称</span><span class="sxs-lookup"><span data-stu-id="4ef7c-126">User principal name of the user to be deleted</span></span>|

## <a name="relationships"></a><span data-ttu-id="4ef7c-127">关系</span><span class="sxs-lookup"><span data-stu-id="4ef7c-127">Relationships</span></span>
<span data-ttu-id="4ef7c-128">无</span><span class="sxs-lookup"><span data-stu-id="4ef7c-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4ef7c-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4ef7c-129">JSON Representation</span></span>
<span data-ttu-id="4ef7c-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4ef7c-130">Here is a JSON representation of the resource.</span></span>
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




