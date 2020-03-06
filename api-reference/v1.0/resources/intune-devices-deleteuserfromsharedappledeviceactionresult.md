---
title: deleteUserFromSharedAppleDeviceActionResult 资源类型
description: 从共享 Apple 设备删除用户操作结果
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 921efba76fa290c104c33544c6801f40aa941dde
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532210"
---
# <a name="deleteuserfromsharedappledeviceactionresult-resource-type"></a><span data-ttu-id="72f6a-103">deleteUserFromSharedAppleDeviceActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="72f6a-103">deleteUserFromSharedAppleDeviceActionResult resource type</span></span>

<span data-ttu-id="72f6a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="72f6a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="72f6a-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="72f6a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="72f6a-106">从共享 Apple 设备删除用户操作结果</span><span class="sxs-lookup"><span data-stu-id="72f6a-106">Delete user from shared apple device action result</span></span>


<span data-ttu-id="72f6a-107">继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="72f6a-107">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="72f6a-108">属性</span><span class="sxs-lookup"><span data-stu-id="72f6a-108">Properties</span></span>
|<span data-ttu-id="72f6a-109">属性</span><span class="sxs-lookup"><span data-stu-id="72f6a-109">Property</span></span>|<span data-ttu-id="72f6a-110">类型</span><span class="sxs-lookup"><span data-stu-id="72f6a-110">Type</span></span>|<span data-ttu-id="72f6a-111">说明</span><span class="sxs-lookup"><span data-stu-id="72f6a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="72f6a-112">actionName</span><span class="sxs-lookup"><span data-stu-id="72f6a-112">actionName</span></span>|<span data-ttu-id="72f6a-113">String</span><span class="sxs-lookup"><span data-stu-id="72f6a-113">String</span></span>|<span data-ttu-id="72f6a-114">操作名称 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="72f6a-114">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="72f6a-115">actionState</span><span class="sxs-lookup"><span data-stu-id="72f6a-115">actionState</span></span>|[<span data-ttu-id="72f6a-116">actionState</span><span class="sxs-lookup"><span data-stu-id="72f6a-116">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="72f6a-117">继承自[deviceActionResult](../resources/intune-devices-deviceactionresult.md)的操作的状态。</span><span class="sxs-lookup"><span data-stu-id="72f6a-117">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="72f6a-118">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed` 或 `notSupported`。</span><span class="sxs-lookup"><span data-stu-id="72f6a-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="72f6a-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="72f6a-119">startDateTime</span></span>|<span data-ttu-id="72f6a-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="72f6a-120">DateTimeOffset</span></span>|<span data-ttu-id="72f6a-121">操作启动的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="72f6a-121">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="72f6a-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="72f6a-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="72f6a-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="72f6a-123">DateTimeOffset</span></span>|<span data-ttu-id="72f6a-124">操作状态上次更新的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="72f6a-124">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="72f6a-125">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="72f6a-125">userPrincipalName</span></span>|<span data-ttu-id="72f6a-126">字符串</span><span class="sxs-lookup"><span data-stu-id="72f6a-126">String</span></span>|<span data-ttu-id="72f6a-127">要删除的用户的用户主体名称</span><span class="sxs-lookup"><span data-stu-id="72f6a-127">User principal name of the user to be deleted</span></span>|

## <a name="relationships"></a><span data-ttu-id="72f6a-128">关系</span><span class="sxs-lookup"><span data-stu-id="72f6a-128">Relationships</span></span>
<span data-ttu-id="72f6a-129">无</span><span class="sxs-lookup"><span data-stu-id="72f6a-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="72f6a-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="72f6a-130">JSON Representation</span></span>
<span data-ttu-id="72f6a-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="72f6a-131">Here is a JSON representation of the resource.</span></span>
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




