---
title: deleteUserFromSharedAppleDeviceActionResult 资源类型
description: 从共享 Apple 设备删除用户操作结果
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2ca29d440f5721e16d13bf91dd366fb9e893108d
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2021
ms.locfileid: "51610961"
---
# <a name="deleteuserfromsharedappledeviceactionresult-resource-type"></a><span data-ttu-id="047f4-103">deleteUserFromSharedAppleDeviceActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="047f4-103">deleteUserFromSharedAppleDeviceActionResult resource type</span></span>

<span data-ttu-id="047f4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="047f4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="047f4-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="047f4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="047f4-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="047f4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="047f4-107">从共享 Apple 设备删除用户操作结果</span><span class="sxs-lookup"><span data-stu-id="047f4-107">Delete user from shared apple device action result</span></span>


<span data-ttu-id="047f4-108">继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="047f4-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="047f4-109">属性</span><span class="sxs-lookup"><span data-stu-id="047f4-109">Properties</span></span>
|<span data-ttu-id="047f4-110">属性</span><span class="sxs-lookup"><span data-stu-id="047f4-110">Property</span></span>|<span data-ttu-id="047f4-111">类型</span><span class="sxs-lookup"><span data-stu-id="047f4-111">Type</span></span>|<span data-ttu-id="047f4-112">Description</span><span class="sxs-lookup"><span data-stu-id="047f4-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="047f4-113">actionName</span><span class="sxs-lookup"><span data-stu-id="047f4-113">actionName</span></span>|<span data-ttu-id="047f4-114">String</span><span class="sxs-lookup"><span data-stu-id="047f4-114">String</span></span>|<span data-ttu-id="047f4-115">操作名称 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="047f4-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="047f4-116">actionState</span><span class="sxs-lookup"><span data-stu-id="047f4-116">actionState</span></span>|[<span data-ttu-id="047f4-117">actionState</span><span class="sxs-lookup"><span data-stu-id="047f4-117">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="047f4-118">操作的状态 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)。</span><span class="sxs-lookup"><span data-stu-id="047f4-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="047f4-119">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed` 或 `notSupported`。</span><span class="sxs-lookup"><span data-stu-id="047f4-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="047f4-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="047f4-120">startDateTime</span></span>|<span data-ttu-id="047f4-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="047f4-121">DateTimeOffset</span></span>|<span data-ttu-id="047f4-122">操作启动的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="047f4-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="047f4-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="047f4-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="047f4-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="047f4-124">DateTimeOffset</span></span>|<span data-ttu-id="047f4-125">操作状态上次更新的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="047f4-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="047f4-126">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="047f4-126">userPrincipalName</span></span>|<span data-ttu-id="047f4-127">String</span><span class="sxs-lookup"><span data-stu-id="047f4-127">String</span></span>|<span data-ttu-id="047f4-128">要删除的用户的用户主体名称</span><span class="sxs-lookup"><span data-stu-id="047f4-128">User principal name of the user to be deleted</span></span>|

## <a name="relationships"></a><span data-ttu-id="047f4-129">关系</span><span class="sxs-lookup"><span data-stu-id="047f4-129">Relationships</span></span>
<span data-ttu-id="047f4-130">无</span><span class="sxs-lookup"><span data-stu-id="047f4-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="047f4-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="047f4-131">JSON Representation</span></span>
<span data-ttu-id="047f4-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="047f4-132">Here is a JSON representation of the resource.</span></span>
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




