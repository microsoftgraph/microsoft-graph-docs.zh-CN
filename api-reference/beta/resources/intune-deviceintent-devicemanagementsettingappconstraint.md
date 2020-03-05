---
title: deviceManagementSettingAppConstraint 资源类型
description: 强制实施设置的约束仅包含 vaild 应用程序类型。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7818493bb5767ce74d0f6f71cf5ffa05a775eded
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42525276"
---
# <a name="devicemanagementsettingappconstraint-resource-type"></a><span data-ttu-id="6332b-103">deviceManagementSettingAppConstraint 资源类型</span><span class="sxs-lookup"><span data-stu-id="6332b-103">deviceManagementSettingAppConstraint resource type</span></span>

<span data-ttu-id="6332b-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="6332b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6332b-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6332b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6332b-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6332b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6332b-107">强制实施设置的约束仅包含 vaild 应用程序类型。</span><span class="sxs-lookup"><span data-stu-id="6332b-107">Constraint enforcing the setting contains only vaild app types.</span></span>


<span data-ttu-id="6332b-108">继承自[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="6332b-108">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6332b-109">属性</span><span class="sxs-lookup"><span data-stu-id="6332b-109">Properties</span></span>
|<span data-ttu-id="6332b-110">属性</span><span class="sxs-lookup"><span data-stu-id="6332b-110">Property</span></span>|<span data-ttu-id="6332b-111">类型</span><span class="sxs-lookup"><span data-stu-id="6332b-111">Type</span></span>|<span data-ttu-id="6332b-112">说明</span><span class="sxs-lookup"><span data-stu-id="6332b-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6332b-113">supportedTypes</span><span class="sxs-lookup"><span data-stu-id="6332b-113">supportedTypes</span></span>|<span data-ttu-id="6332b-114">String 集合</span><span class="sxs-lookup"><span data-stu-id="6332b-114">String collection</span></span>|<span data-ttu-id="6332b-115">允许此设置的可接受的应用程序类型</span><span class="sxs-lookup"><span data-stu-id="6332b-115">Acceptable app types to allow for this setting</span></span>|

## <a name="relationships"></a><span data-ttu-id="6332b-116">关系</span><span class="sxs-lookup"><span data-stu-id="6332b-116">Relationships</span></span>
<span data-ttu-id="6332b-117">无</span><span class="sxs-lookup"><span data-stu-id="6332b-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6332b-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6332b-118">JSON Representation</span></span>
<span data-ttu-id="6332b-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6332b-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettingAppConstraint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingAppConstraint",
  "supportedTypes": [
    "String"
  ]
}
```



