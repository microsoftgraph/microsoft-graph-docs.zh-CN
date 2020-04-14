---
title: deleteUserFromSharedAppleDeviceActionResult 资源类型
description: 从共享 Apple 设备删除用户操作结果
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8206383e33ff0fa7a682485fe63d1ec978aa9e68
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43456883"
---
# <a name="deleteuserfromsharedappledeviceactionresult-resource-type"></a><span data-ttu-id="ecc94-103">deleteUserFromSharedAppleDeviceActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="ecc94-103">deleteUserFromSharedAppleDeviceActionResult resource type</span></span>

<span data-ttu-id="ecc94-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ecc94-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ecc94-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ecc94-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ecc94-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ecc94-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ecc94-107">从共享 Apple 设备删除用户操作结果</span><span class="sxs-lookup"><span data-stu-id="ecc94-107">Delete user from shared apple device action result</span></span>


<span data-ttu-id="ecc94-108">继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="ecc94-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ecc94-109">属性</span><span class="sxs-lookup"><span data-stu-id="ecc94-109">Properties</span></span>
|<span data-ttu-id="ecc94-110">属性</span><span class="sxs-lookup"><span data-stu-id="ecc94-110">Property</span></span>|<span data-ttu-id="ecc94-111">类型</span><span class="sxs-lookup"><span data-stu-id="ecc94-111">Type</span></span>|<span data-ttu-id="ecc94-112">说明</span><span class="sxs-lookup"><span data-stu-id="ecc94-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ecc94-113">actionName</span><span class="sxs-lookup"><span data-stu-id="ecc94-113">actionName</span></span>|<span data-ttu-id="ecc94-114">String</span><span class="sxs-lookup"><span data-stu-id="ecc94-114">String</span></span>|<span data-ttu-id="ecc94-115">操作名称 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="ecc94-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="ecc94-116">actionState</span><span class="sxs-lookup"><span data-stu-id="ecc94-116">actionState</span></span>|[<span data-ttu-id="ecc94-117">actionState</span><span class="sxs-lookup"><span data-stu-id="ecc94-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="ecc94-118">继承自[deviceActionResult](../resources/intune-devices-deviceactionresult.md)的操作的状态。</span><span class="sxs-lookup"><span data-stu-id="ecc94-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="ecc94-119">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed` 或 `notSupported`。</span><span class="sxs-lookup"><span data-stu-id="ecc94-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="ecc94-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="ecc94-120">startDateTime</span></span>|<span data-ttu-id="ecc94-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ecc94-121">DateTimeOffset</span></span>|<span data-ttu-id="ecc94-122">操作启动的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="ecc94-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="ecc94-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="ecc94-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="ecc94-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ecc94-124">DateTimeOffset</span></span>|<span data-ttu-id="ecc94-125">操作状态上次更新的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="ecc94-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="ecc94-126">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ecc94-126">userPrincipalName</span></span>|<span data-ttu-id="ecc94-127">String</span><span class="sxs-lookup"><span data-stu-id="ecc94-127">String</span></span>|<span data-ttu-id="ecc94-128">要删除的用户的用户主体名称</span><span class="sxs-lookup"><span data-stu-id="ecc94-128">User principal name of the user to be deleted</span></span>|

## <a name="relationships"></a><span data-ttu-id="ecc94-129">关系</span><span class="sxs-lookup"><span data-stu-id="ecc94-129">Relationships</span></span>
<span data-ttu-id="ecc94-130">无</span><span class="sxs-lookup"><span data-stu-id="ecc94-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ecc94-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ecc94-131">JSON Representation</span></span>
<span data-ttu-id="ecc94-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ecc94-132">Here is a JSON representation of the resource.</span></span>
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



