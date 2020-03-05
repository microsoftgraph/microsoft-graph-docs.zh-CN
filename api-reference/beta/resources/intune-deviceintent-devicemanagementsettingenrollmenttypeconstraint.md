---
title: deviceManagementSettingEnrollmentTypeConstraint 资源类型
description: 强制实施应用于设置的注册类型的约束
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: cfea5505dc05ac037ced5d9b714edb53ed6f768d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528797"
---
# <a name="devicemanagementsettingenrollmenttypeconstraint-resource-type"></a><span data-ttu-id="b2a55-103">deviceManagementSettingEnrollmentTypeConstraint 资源类型</span><span class="sxs-lookup"><span data-stu-id="b2a55-103">deviceManagementSettingEnrollmentTypeConstraint resource type</span></span>

<span data-ttu-id="b2a55-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="b2a55-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b2a55-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b2a55-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b2a55-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b2a55-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b2a55-107">强制实施应用于设置的注册类型的约束</span><span class="sxs-lookup"><span data-stu-id="b2a55-107">Constraint that enforces the enrollment types applied to a setting</span></span>


<span data-ttu-id="b2a55-108">继承自[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="b2a55-108">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b2a55-109">属性</span><span class="sxs-lookup"><span data-stu-id="b2a55-109">Properties</span></span>
|<span data-ttu-id="b2a55-110">属性</span><span class="sxs-lookup"><span data-stu-id="b2a55-110">Property</span></span>|<span data-ttu-id="b2a55-111">类型</span><span class="sxs-lookup"><span data-stu-id="b2a55-111">Type</span></span>|<span data-ttu-id="b2a55-112">说明</span><span class="sxs-lookup"><span data-stu-id="b2a55-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b2a55-113">enrollmentTypes</span><span class="sxs-lookup"><span data-stu-id="b2a55-113">enrollmentTypes</span></span>|<span data-ttu-id="b2a55-114">String 集合</span><span class="sxs-lookup"><span data-stu-id="b2a55-114">String collection</span></span>|<span data-ttu-id="b2a55-115">注册类型列表</span><span class="sxs-lookup"><span data-stu-id="b2a55-115">List of enrollment types</span></span>|

## <a name="relationships"></a><span data-ttu-id="b2a55-116">关系</span><span class="sxs-lookup"><span data-stu-id="b2a55-116">Relationships</span></span>
<span data-ttu-id="b2a55-117">无</span><span class="sxs-lookup"><span data-stu-id="b2a55-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b2a55-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b2a55-118">JSON Representation</span></span>
<span data-ttu-id="b2a55-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b2a55-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettingEnrollmentTypeConstraint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingEnrollmentTypeConstraint",
  "enrollmentTypes": [
    "String"
  ]
}
```



