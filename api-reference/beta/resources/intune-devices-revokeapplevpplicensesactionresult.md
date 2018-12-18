---
title: revokeAppleVppLicensesActionResult 资源类型
description: 取消 Apple Vpp 许可证操作结果
author: tfitzmac
ms.openlocfilehash: b45a2ddec46ddc5cac47937cb776d0f0da6c64a8
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27361045"
---
# <a name="revokeapplevpplicensesactionresult-resource-type"></a><span data-ttu-id="0b018-103">revokeAppleVppLicensesActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="0b018-103">revokeAppleVppLicensesActionResult resource type</span></span>

> <span data-ttu-id="0b018-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="0b018-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0b018-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="0b018-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0b018-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="0b018-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0b018-107">取消 Apple Vpp 许可证操作结果</span><span class="sxs-lookup"><span data-stu-id="0b018-107">Revoke Apple Vpp licenses action result</span></span>

<span data-ttu-id="0b018-108">继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="0b018-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0b018-109">属性</span><span class="sxs-lookup"><span data-stu-id="0b018-109">Properties</span></span>
|<span data-ttu-id="0b018-110">属性</span><span class="sxs-lookup"><span data-stu-id="0b018-110">Property</span></span>|<span data-ttu-id="0b018-111">类型</span><span class="sxs-lookup"><span data-stu-id="0b018-111">Type</span></span>|<span data-ttu-id="0b018-112">说明</span><span class="sxs-lookup"><span data-stu-id="0b018-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0b018-113">actionName</span><span class="sxs-lookup"><span data-stu-id="0b018-113">actionName</span></span>|<span data-ttu-id="0b018-114">String</span><span class="sxs-lookup"><span data-stu-id="0b018-114">String</span></span>|<span data-ttu-id="0b018-115">操作名称 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="0b018-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="0b018-116">actionState</span><span class="sxs-lookup"><span data-stu-id="0b018-116">actionState</span></span>|[<span data-ttu-id="0b018-117">actionState</span><span class="sxs-lookup"><span data-stu-id="0b018-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="0b018-118">从[deviceActionResult](../resources/intune-devices-deviceactionresult.md)继承操作的状态。</span><span class="sxs-lookup"><span data-stu-id="0b018-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="0b018-119">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported`。</span><span class="sxs-lookup"><span data-stu-id="0b018-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="0b018-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="0b018-120">startDateTime</span></span>|<span data-ttu-id="0b018-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0b018-121">DateTimeOffset</span></span>|<span data-ttu-id="0b018-122">启动操作的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="0b018-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="0b018-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="0b018-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="0b018-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0b018-124">DateTimeOffset</span></span>|<span data-ttu-id="0b018-125">上次更新操作状态的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="0b018-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="0b018-126">totalLicensesCount</span><span class="sxs-lookup"><span data-stu-id="0b018-126">totalLicensesCount</span></span>|<span data-ttu-id="0b018-127">Int32</span><span class="sxs-lookup"><span data-stu-id="0b018-127">Int32</span></span>|<span data-ttu-id="0b018-128">Apple Vpp 许可证关联总数</span><span class="sxs-lookup"><span data-stu-id="0b018-128">Total number of Apple Vpp licenses associated</span></span>|
|<span data-ttu-id="0b018-129">failedLicensesCount</span><span class="sxs-lookup"><span data-stu-id="0b018-129">failedLicensesCount</span></span>|<span data-ttu-id="0b018-130">Int32</span><span class="sxs-lookup"><span data-stu-id="0b018-130">Int32</span></span>|<span data-ttu-id="0b018-131">无法撤消的 Apple Vpp 许可证的总数</span><span class="sxs-lookup"><span data-stu-id="0b018-131">Total number of Apple Vpp licenses that failed to revoke</span></span>|

## <a name="relationships"></a><span data-ttu-id="0b018-132">Relationships</span><span class="sxs-lookup"><span data-stu-id="0b018-132">Relationships</span></span>
<span data-ttu-id="0b018-133">无</span><span class="sxs-lookup"><span data-stu-id="0b018-133">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0b018-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0b018-134">JSON Representation</span></span>
<span data-ttu-id="0b018-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0b018-135">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.revokeAppleVppLicensesActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.revokeAppleVppLicensesActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "totalLicensesCount": 1024,
  "failedLicensesCount": 1024
}
```





