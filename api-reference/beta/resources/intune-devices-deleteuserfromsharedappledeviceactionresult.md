---
title: deleteUserFromSharedAppleDeviceActionResult 资源类型
description: 从共享 Apple 设备删除用户操作结果
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 797c5505f52a9f042ef8fdff615f1e7a1ae9b73a
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48703641"
---
# <a name="deleteuserfromsharedappledeviceactionresult-resource-type"></a><span data-ttu-id="8de85-103">deleteUserFromSharedAppleDeviceActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="8de85-103">deleteUserFromSharedAppleDeviceActionResult resource type</span></span>

<span data-ttu-id="8de85-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8de85-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8de85-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8de85-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8de85-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8de85-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8de85-107">从共享 Apple 设备删除用户操作结果</span><span class="sxs-lookup"><span data-stu-id="8de85-107">Delete user from shared apple device action result</span></span>


<span data-ttu-id="8de85-108">继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="8de85-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8de85-109">属性</span><span class="sxs-lookup"><span data-stu-id="8de85-109">Properties</span></span>
|<span data-ttu-id="8de85-110">属性</span><span class="sxs-lookup"><span data-stu-id="8de85-110">Property</span></span>|<span data-ttu-id="8de85-111">类型</span><span class="sxs-lookup"><span data-stu-id="8de85-111">Type</span></span>|<span data-ttu-id="8de85-112">说明</span><span class="sxs-lookup"><span data-stu-id="8de85-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8de85-113">actionName</span><span class="sxs-lookup"><span data-stu-id="8de85-113">actionName</span></span>|<span data-ttu-id="8de85-114">String</span><span class="sxs-lookup"><span data-stu-id="8de85-114">String</span></span>|<span data-ttu-id="8de85-115">操作名称 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="8de85-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="8de85-116">actionState</span><span class="sxs-lookup"><span data-stu-id="8de85-116">actionState</span></span>|[<span data-ttu-id="8de85-117">actionState</span><span class="sxs-lookup"><span data-stu-id="8de85-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="8de85-118">继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)的操作的状态。</span><span class="sxs-lookup"><span data-stu-id="8de85-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="8de85-119">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed` 或 `notSupported`。</span><span class="sxs-lookup"><span data-stu-id="8de85-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="8de85-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="8de85-120">startDateTime</span></span>|<span data-ttu-id="8de85-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8de85-121">DateTimeOffset</span></span>|<span data-ttu-id="8de85-122">操作启动的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="8de85-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="8de85-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="8de85-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="8de85-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8de85-124">DateTimeOffset</span></span>|<span data-ttu-id="8de85-125">操作状态上次更新的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="8de85-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="8de85-126">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="8de85-126">userPrincipalName</span></span>|<span data-ttu-id="8de85-127">String</span><span class="sxs-lookup"><span data-stu-id="8de85-127">String</span></span>|<span data-ttu-id="8de85-128">要删除的用户的用户主体名称</span><span class="sxs-lookup"><span data-stu-id="8de85-128">User principal name of the user to be deleted</span></span>|

## <a name="relationships"></a><span data-ttu-id="8de85-129">关系</span><span class="sxs-lookup"><span data-stu-id="8de85-129">Relationships</span></span>
<span data-ttu-id="8de85-130">无</span><span class="sxs-lookup"><span data-stu-id="8de85-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8de85-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8de85-131">JSON Representation</span></span>
<span data-ttu-id="8de85-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8de85-132">Here is a JSON representation of the resource.</span></span>
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





