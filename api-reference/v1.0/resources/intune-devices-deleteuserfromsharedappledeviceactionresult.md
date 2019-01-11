---
title: deleteUserFromSharedAppleDeviceActionResult 资源类型
description: 从共享 Apple 设备删除用户操作结果
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 1c6e014f0461c1e6a72a4d67791c27dc401f87f6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27804947"
---
# <a name="deleteuserfromsharedappledeviceactionresult-resource-type"></a><span data-ttu-id="c1bee-103">deleteUserFromSharedAppleDeviceActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="c1bee-103">deleteUserFromSharedAppleDeviceActionResult resource type</span></span>

> <span data-ttu-id="c1bee-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="c1bee-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c1bee-105">从共享 Apple 设备删除用户操作结果</span><span class="sxs-lookup"><span data-stu-id="c1bee-105">Delete user from shared apple device action result</span></span>

<span data-ttu-id="c1bee-106">继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="c1bee-106">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c1bee-107">属性</span><span class="sxs-lookup"><span data-stu-id="c1bee-107">Properties</span></span>
|<span data-ttu-id="c1bee-108">属性</span><span class="sxs-lookup"><span data-stu-id="c1bee-108">Property</span></span>|<span data-ttu-id="c1bee-109">类型</span><span class="sxs-lookup"><span data-stu-id="c1bee-109">Type</span></span>|<span data-ttu-id="c1bee-110">说明</span><span class="sxs-lookup"><span data-stu-id="c1bee-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1bee-111">actionName</span><span class="sxs-lookup"><span data-stu-id="c1bee-111">actionName</span></span>|<span data-ttu-id="c1bee-112">String</span><span class="sxs-lookup"><span data-stu-id="c1bee-112">String</span></span>|<span data-ttu-id="c1bee-113">操作名称 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="c1bee-113">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="c1bee-114">actionState</span><span class="sxs-lookup"><span data-stu-id="c1bee-114">actionState</span></span>|[<span data-ttu-id="c1bee-115">actionState</span><span class="sxs-lookup"><span data-stu-id="c1bee-115">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="c1bee-116">从[deviceActionResult](../resources/intune-devices-deviceactionresult.md)继承操作的状态。</span><span class="sxs-lookup"><span data-stu-id="c1bee-116">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="c1bee-117">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported`。</span><span class="sxs-lookup"><span data-stu-id="c1bee-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="c1bee-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="c1bee-118">startDateTime</span></span>|<span data-ttu-id="c1bee-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c1bee-119">DateTimeOffset</span></span>|<span data-ttu-id="c1bee-120">启动操作的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="c1bee-120">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="c1bee-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="c1bee-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="c1bee-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c1bee-122">DateTimeOffset</span></span>|<span data-ttu-id="c1bee-123">操作状态上次更新的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="c1bee-123">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="c1bee-124">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c1bee-124">userPrincipalName</span></span>|<span data-ttu-id="c1bee-125">String</span><span class="sxs-lookup"><span data-stu-id="c1bee-125">String</span></span>|<span data-ttu-id="c1bee-126">要删除的用户的用户主体名称</span><span class="sxs-lookup"><span data-stu-id="c1bee-126">User principal name of the user to be deleted</span></span>|

## <a name="relationships"></a><span data-ttu-id="c1bee-127">关系</span><span class="sxs-lookup"><span data-stu-id="c1bee-127">Relationships</span></span>
<span data-ttu-id="c1bee-128">无</span><span class="sxs-lookup"><span data-stu-id="c1bee-128">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c1bee-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c1bee-129">JSON Representation</span></span>
<span data-ttu-id="c1bee-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c1bee-130">Here is a JSON representation of the resource.</span></span>
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



