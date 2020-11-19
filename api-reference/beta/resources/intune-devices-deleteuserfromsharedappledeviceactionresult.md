---
title: deleteUserFromSharedAppleDeviceActionResult 资源类型
description: 从共享 Apple 设备删除用户操作结果
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e8193551aed2a3604f79978d3907c9af6728b6eb
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49267829"
---
# <a name="deleteuserfromsharedappledeviceactionresult-resource-type"></a><span data-ttu-id="615c2-103">deleteUserFromSharedAppleDeviceActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="615c2-103">deleteUserFromSharedAppleDeviceActionResult resource type</span></span>

<span data-ttu-id="615c2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="615c2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="615c2-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="615c2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="615c2-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="615c2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="615c2-107">从共享 Apple 设备删除用户操作结果</span><span class="sxs-lookup"><span data-stu-id="615c2-107">Delete user from shared apple device action result</span></span>


<span data-ttu-id="615c2-108">继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="615c2-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="615c2-109">属性</span><span class="sxs-lookup"><span data-stu-id="615c2-109">Properties</span></span>
|<span data-ttu-id="615c2-110">属性</span><span class="sxs-lookup"><span data-stu-id="615c2-110">Property</span></span>|<span data-ttu-id="615c2-111">类型</span><span class="sxs-lookup"><span data-stu-id="615c2-111">Type</span></span>|<span data-ttu-id="615c2-112">说明</span><span class="sxs-lookup"><span data-stu-id="615c2-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="615c2-113">actionName</span><span class="sxs-lookup"><span data-stu-id="615c2-113">actionName</span></span>|<span data-ttu-id="615c2-114">String</span><span class="sxs-lookup"><span data-stu-id="615c2-114">String</span></span>|<span data-ttu-id="615c2-115">操作名称 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="615c2-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="615c2-116">actionState</span><span class="sxs-lookup"><span data-stu-id="615c2-116">actionState</span></span>|[<span data-ttu-id="615c2-117">actionState</span><span class="sxs-lookup"><span data-stu-id="615c2-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="615c2-118">继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)的操作的状态。</span><span class="sxs-lookup"><span data-stu-id="615c2-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="615c2-119">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed` 或 `notSupported`。</span><span class="sxs-lookup"><span data-stu-id="615c2-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="615c2-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="615c2-120">startDateTime</span></span>|<span data-ttu-id="615c2-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="615c2-121">DateTimeOffset</span></span>|<span data-ttu-id="615c2-122">操作启动的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="615c2-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="615c2-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="615c2-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="615c2-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="615c2-124">DateTimeOffset</span></span>|<span data-ttu-id="615c2-125">操作状态上次更新的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="615c2-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="615c2-126">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="615c2-126">userPrincipalName</span></span>|<span data-ttu-id="615c2-127">字符串</span><span class="sxs-lookup"><span data-stu-id="615c2-127">String</span></span>|<span data-ttu-id="615c2-128">要删除的用户的用户主体名称</span><span class="sxs-lookup"><span data-stu-id="615c2-128">User principal name of the user to be deleted</span></span>|

## <a name="relationships"></a><span data-ttu-id="615c2-129">关系</span><span class="sxs-lookup"><span data-stu-id="615c2-129">Relationships</span></span>
<span data-ttu-id="615c2-130">无</span><span class="sxs-lookup"><span data-stu-id="615c2-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="615c2-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="615c2-131">JSON Representation</span></span>
<span data-ttu-id="615c2-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="615c2-132">Here is a JSON representation of the resource.</span></span>
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




