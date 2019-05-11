---
title: deleteUserFromSharedAppleDeviceActionResult 资源类型
description: 从共享 Apple 设备删除用户操作结果
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4a86128b3bb8f863c21225567c91dc0a9938bc7b
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33942176"
---
# <a name="deleteuserfromsharedappledeviceactionresult-resource-type"></a><span data-ttu-id="fba1b-103">deleteUserFromSharedAppleDeviceActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="fba1b-103">deleteUserFromSharedAppleDeviceActionResult resource type</span></span>

> <span data-ttu-id="fba1b-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="fba1b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fba1b-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fba1b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fba1b-106">从共享 Apple 设备删除用户操作结果</span><span class="sxs-lookup"><span data-stu-id="fba1b-106">Delete user from shared apple device action result</span></span>


<span data-ttu-id="fba1b-107">继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="fba1b-107">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="fba1b-108">属性</span><span class="sxs-lookup"><span data-stu-id="fba1b-108">Properties</span></span>
|<span data-ttu-id="fba1b-109">属性</span><span class="sxs-lookup"><span data-stu-id="fba1b-109">Property</span></span>|<span data-ttu-id="fba1b-110">类型</span><span class="sxs-lookup"><span data-stu-id="fba1b-110">Type</span></span>|<span data-ttu-id="fba1b-111">说明</span><span class="sxs-lookup"><span data-stu-id="fba1b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fba1b-112">actionName</span><span class="sxs-lookup"><span data-stu-id="fba1b-112">actionName</span></span>|<span data-ttu-id="fba1b-113">String</span><span class="sxs-lookup"><span data-stu-id="fba1b-113">String</span></span>|<span data-ttu-id="fba1b-114">操作名称 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="fba1b-114">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="fba1b-115">actionState</span><span class="sxs-lookup"><span data-stu-id="fba1b-115">actionState</span></span>|[<span data-ttu-id="fba1b-116">actionState</span><span class="sxs-lookup"><span data-stu-id="fba1b-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="fba1b-117">继承自[deviceActionResult](../resources/intune-devices-deviceactionresult.md)的操作的状态。</span><span class="sxs-lookup"><span data-stu-id="fba1b-117">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="fba1b-118">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed` 或 `notSupported`。</span><span class="sxs-lookup"><span data-stu-id="fba1b-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="fba1b-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="fba1b-119">startDateTime</span></span>|<span data-ttu-id="fba1b-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fba1b-120">DateTimeOffset</span></span>|<span data-ttu-id="fba1b-121">操作启动的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="fba1b-121">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="fba1b-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="fba1b-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="fba1b-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fba1b-123">DateTimeOffset</span></span>|<span data-ttu-id="fba1b-124">操作状态上次更新的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="fba1b-124">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="fba1b-125">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="fba1b-125">userPrincipalName</span></span>|<span data-ttu-id="fba1b-126">String</span><span class="sxs-lookup"><span data-stu-id="fba1b-126">String</span></span>|<span data-ttu-id="fba1b-127">要删除的用户的用户主体名称</span><span class="sxs-lookup"><span data-stu-id="fba1b-127">User principal name of the user to be deleted</span></span>|

## <a name="relationships"></a><span data-ttu-id="fba1b-128">关系</span><span class="sxs-lookup"><span data-stu-id="fba1b-128">Relationships</span></span>
<span data-ttu-id="fba1b-129">无</span><span class="sxs-lookup"><span data-stu-id="fba1b-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fba1b-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fba1b-130">JSON Representation</span></span>
<span data-ttu-id="fba1b-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fba1b-131">Here is a JSON representation of the resource.</span></span>
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




