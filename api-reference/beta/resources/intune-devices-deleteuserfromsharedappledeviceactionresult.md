---
title: deleteUserFromSharedAppleDeviceActionResult 资源类型
description: 从共享 Apple 设备删除用户操作结果
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 90dec4f79d44d4441d23bdba649ddeb3caa311a7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32454028"
---
# <a name="deleteuserfromsharedappledeviceactionresult-resource-type"></a><span data-ttu-id="2e5ad-103">deleteUserFromSharedAppleDeviceActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="2e5ad-103">deleteUserFromSharedAppleDeviceActionResult resource type</span></span>

> <span data-ttu-id="2e5ad-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2e5ad-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2e5ad-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2e5ad-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2e5ad-106">从共享 Apple 设备删除用户操作结果</span><span class="sxs-lookup"><span data-stu-id="2e5ad-106">Delete user from shared apple device action result</span></span>


<span data-ttu-id="2e5ad-107">继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="2e5ad-107">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="2e5ad-108">属性</span><span class="sxs-lookup"><span data-stu-id="2e5ad-108">Properties</span></span>
|<span data-ttu-id="2e5ad-109">属性</span><span class="sxs-lookup"><span data-stu-id="2e5ad-109">Property</span></span>|<span data-ttu-id="2e5ad-110">类型</span><span class="sxs-lookup"><span data-stu-id="2e5ad-110">Type</span></span>|<span data-ttu-id="2e5ad-111">描述</span><span class="sxs-lookup"><span data-stu-id="2e5ad-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2e5ad-112">actionName</span><span class="sxs-lookup"><span data-stu-id="2e5ad-112">actionName</span></span>|<span data-ttu-id="2e5ad-113">String</span><span class="sxs-lookup"><span data-stu-id="2e5ad-113">String</span></span>|<span data-ttu-id="2e5ad-114">操作名称 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="2e5ad-114">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="2e5ad-115">actionState</span><span class="sxs-lookup"><span data-stu-id="2e5ad-115">actionState</span></span>|[<span data-ttu-id="2e5ad-116">actionState</span><span class="sxs-lookup"><span data-stu-id="2e5ad-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="2e5ad-117">继承自[deviceActionResult](../resources/intune-devices-deviceactionresult.md)的操作的状态。</span><span class="sxs-lookup"><span data-stu-id="2e5ad-117">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="2e5ad-118">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed` 或 `notSupported`。</span><span class="sxs-lookup"><span data-stu-id="2e5ad-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="2e5ad-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="2e5ad-119">startDateTime</span></span>|<span data-ttu-id="2e5ad-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2e5ad-120">DateTimeOffset</span></span>|<span data-ttu-id="2e5ad-121">操作启动的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="2e5ad-121">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="2e5ad-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="2e5ad-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="2e5ad-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2e5ad-123">DateTimeOffset</span></span>|<span data-ttu-id="2e5ad-124">操作状态上次更新的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="2e5ad-124">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="2e5ad-125">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="2e5ad-125">userPrincipalName</span></span>|<span data-ttu-id="2e5ad-126">String</span><span class="sxs-lookup"><span data-stu-id="2e5ad-126">String</span></span>|<span data-ttu-id="2e5ad-127">要删除的用户的用户主体名称</span><span class="sxs-lookup"><span data-stu-id="2e5ad-127">User principal name of the user to be deleted</span></span>|

## <a name="relationships"></a><span data-ttu-id="2e5ad-128">关系</span><span class="sxs-lookup"><span data-stu-id="2e5ad-128">Relationships</span></span>
<span data-ttu-id="2e5ad-129">无</span><span class="sxs-lookup"><span data-stu-id="2e5ad-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2e5ad-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2e5ad-130">JSON Representation</span></span>
<span data-ttu-id="2e5ad-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2e5ad-131">Here is a JSON representation of the resource.</span></span>
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





