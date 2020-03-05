---
title: deleteUserFromSharedAppleDeviceActionResult 资源类型
description: 从共享 Apple 设备删除用户操作结果
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 82decf5af685014560ce5a5b7a66fee7cede41c7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528662"
---
# <a name="deleteuserfromsharedappledeviceactionresult-resource-type"></a><span data-ttu-id="1ed36-103">deleteUserFromSharedAppleDeviceActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="1ed36-103">deleteUserFromSharedAppleDeviceActionResult resource type</span></span>

<span data-ttu-id="1ed36-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="1ed36-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1ed36-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1ed36-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1ed36-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1ed36-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1ed36-107">从共享 Apple 设备删除用户操作结果</span><span class="sxs-lookup"><span data-stu-id="1ed36-107">Delete user from shared apple device action result</span></span>


<span data-ttu-id="1ed36-108">继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="1ed36-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1ed36-109">属性</span><span class="sxs-lookup"><span data-stu-id="1ed36-109">Properties</span></span>
|<span data-ttu-id="1ed36-110">属性</span><span class="sxs-lookup"><span data-stu-id="1ed36-110">Property</span></span>|<span data-ttu-id="1ed36-111">类型</span><span class="sxs-lookup"><span data-stu-id="1ed36-111">Type</span></span>|<span data-ttu-id="1ed36-112">说明</span><span class="sxs-lookup"><span data-stu-id="1ed36-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1ed36-113">actionName</span><span class="sxs-lookup"><span data-stu-id="1ed36-113">actionName</span></span>|<span data-ttu-id="1ed36-114">String</span><span class="sxs-lookup"><span data-stu-id="1ed36-114">String</span></span>|<span data-ttu-id="1ed36-115">操作名称 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="1ed36-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="1ed36-116">actionState</span><span class="sxs-lookup"><span data-stu-id="1ed36-116">actionState</span></span>|[<span data-ttu-id="1ed36-117">actionState</span><span class="sxs-lookup"><span data-stu-id="1ed36-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="1ed36-118">继承自[deviceActionResult](../resources/intune-devices-deviceactionresult.md)的操作的状态。</span><span class="sxs-lookup"><span data-stu-id="1ed36-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="1ed36-119">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed` 或 `notSupported`。</span><span class="sxs-lookup"><span data-stu-id="1ed36-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="1ed36-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="1ed36-120">startDateTime</span></span>|<span data-ttu-id="1ed36-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1ed36-121">DateTimeOffset</span></span>|<span data-ttu-id="1ed36-122">操作启动的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="1ed36-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="1ed36-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="1ed36-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="1ed36-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1ed36-124">DateTimeOffset</span></span>|<span data-ttu-id="1ed36-125">操作状态上次更新的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="1ed36-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="1ed36-126">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="1ed36-126">userPrincipalName</span></span>|<span data-ttu-id="1ed36-127">String</span><span class="sxs-lookup"><span data-stu-id="1ed36-127">String</span></span>|<span data-ttu-id="1ed36-128">要删除的用户的用户主体名称</span><span class="sxs-lookup"><span data-stu-id="1ed36-128">User principal name of the user to be deleted</span></span>|

## <a name="relationships"></a><span data-ttu-id="1ed36-129">关系</span><span class="sxs-lookup"><span data-stu-id="1ed36-129">Relationships</span></span>
<span data-ttu-id="1ed36-130">无</span><span class="sxs-lookup"><span data-stu-id="1ed36-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1ed36-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1ed36-131">JSON Representation</span></span>
<span data-ttu-id="1ed36-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1ed36-132">Here is a JSON representation of the resource.</span></span>
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



