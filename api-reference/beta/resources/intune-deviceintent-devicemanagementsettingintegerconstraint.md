---
title: deviceManagementSettingIntegerConstraint 资源类型
description: 强制整数设置允许的值范围的约束
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9bf28c3f3942e99841b43f1cd7ff5304fd81d800
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32550684"
---
# <a name="devicemanagementsettingintegerconstraint-resource-type"></a><span data-ttu-id="d56ec-103">deviceManagementSettingIntegerConstraint 资源类型</span><span class="sxs-lookup"><span data-stu-id="d56ec-103">deviceManagementSettingIntegerConstraint resource type</span></span>

> <span data-ttu-id="d56ec-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d56ec-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d56ec-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d56ec-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d56ec-106">强制整数设置允许的值范围的约束</span><span class="sxs-lookup"><span data-stu-id="d56ec-106">Constraint enforcing the permitted value range for an integer setting</span></span>


<span data-ttu-id="d56ec-107">继承自[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="d56ec-107">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d56ec-108">属性</span><span class="sxs-lookup"><span data-stu-id="d56ec-108">Properties</span></span>
|<span data-ttu-id="d56ec-109">属性</span><span class="sxs-lookup"><span data-stu-id="d56ec-109">Property</span></span>|<span data-ttu-id="d56ec-110">类型</span><span class="sxs-lookup"><span data-stu-id="d56ec-110">Type</span></span>|<span data-ttu-id="d56ec-111">说明</span><span class="sxs-lookup"><span data-stu-id="d56ec-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d56ec-112">minimumValue</span><span class="sxs-lookup"><span data-stu-id="d56ec-112">minimumValue</span></span>|<span data-ttu-id="d56ec-113">Int32</span><span class="sxs-lookup"><span data-stu-id="d56ec-113">Int32</span></span>|<span data-ttu-id="d56ec-114">允许的最小值</span><span class="sxs-lookup"><span data-stu-id="d56ec-114">The minimum permitted value</span></span>|
|<span data-ttu-id="d56ec-115">maximumValue</span><span class="sxs-lookup"><span data-stu-id="d56ec-115">maximumValue</span></span>|<span data-ttu-id="d56ec-116">Int32</span><span class="sxs-lookup"><span data-stu-id="d56ec-116">Int32</span></span>|<span data-ttu-id="d56ec-117">允许的最大值</span><span class="sxs-lookup"><span data-stu-id="d56ec-117">The maximum permitted value</span></span>|

## <a name="relationships"></a><span data-ttu-id="d56ec-118">关系</span><span class="sxs-lookup"><span data-stu-id="d56ec-118">Relationships</span></span>
<span data-ttu-id="d56ec-119">无</span><span class="sxs-lookup"><span data-stu-id="d56ec-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d56ec-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d56ec-120">JSON Representation</span></span>
<span data-ttu-id="d56ec-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d56ec-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettingIntegerConstraint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingIntegerConstraint",
  "minimumValue": 1024,
  "maximumValue": 1024
}
```





