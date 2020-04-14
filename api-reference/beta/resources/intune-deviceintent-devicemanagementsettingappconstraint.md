---
title: deviceManagementSettingAppConstraint 资源类型
description: 强制实施设置的约束仅包含 vaild 应用程序类型。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 012f20e69f79018ffecbac0ff4558687ec407bdd
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43443318"
---
# <a name="devicemanagementsettingappconstraint-resource-type"></a><span data-ttu-id="88419-103">deviceManagementSettingAppConstraint 资源类型</span><span class="sxs-lookup"><span data-stu-id="88419-103">deviceManagementSettingAppConstraint resource type</span></span>

<span data-ttu-id="88419-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="88419-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="88419-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="88419-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="88419-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="88419-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="88419-107">强制实施设置的约束仅包含 vaild 应用程序类型。</span><span class="sxs-lookup"><span data-stu-id="88419-107">Constraint enforcing the setting contains only vaild app types.</span></span>


<span data-ttu-id="88419-108">继承自[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="88419-108">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="88419-109">属性</span><span class="sxs-lookup"><span data-stu-id="88419-109">Properties</span></span>
|<span data-ttu-id="88419-110">属性</span><span class="sxs-lookup"><span data-stu-id="88419-110">Property</span></span>|<span data-ttu-id="88419-111">类型</span><span class="sxs-lookup"><span data-stu-id="88419-111">Type</span></span>|<span data-ttu-id="88419-112">说明</span><span class="sxs-lookup"><span data-stu-id="88419-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88419-113">supportedTypes</span><span class="sxs-lookup"><span data-stu-id="88419-113">supportedTypes</span></span>|<span data-ttu-id="88419-114">String 集合</span><span class="sxs-lookup"><span data-stu-id="88419-114">String collection</span></span>|<span data-ttu-id="88419-115">允许此设置的可接受的应用程序类型</span><span class="sxs-lookup"><span data-stu-id="88419-115">Acceptable app types to allow for this setting</span></span>|

## <a name="relationships"></a><span data-ttu-id="88419-116">关系</span><span class="sxs-lookup"><span data-stu-id="88419-116">Relationships</span></span>
<span data-ttu-id="88419-117">无</span><span class="sxs-lookup"><span data-stu-id="88419-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="88419-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="88419-118">JSON Representation</span></span>
<span data-ttu-id="88419-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="88419-119">Here is a JSON representation of the resource.</span></span>
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



