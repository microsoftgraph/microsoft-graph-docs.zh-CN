---
title: deviceManagementSettingFileConstraint 资源类型
description: 强制实施文件扩展名的约束可接受给定设置
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1757f3d6d7e6e60a9c45e95e531a142fabbb95f0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42525248"
---
# <a name="devicemanagementsettingfileconstraint-resource-type"></a><span data-ttu-id="fc525-103">deviceManagementSettingFileConstraint 资源类型</span><span class="sxs-lookup"><span data-stu-id="fc525-103">deviceManagementSettingFileConstraint resource type</span></span>

<span data-ttu-id="fc525-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="fc525-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fc525-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="fc525-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fc525-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fc525-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fc525-107">强制实施文件扩展名的约束可接受给定设置</span><span class="sxs-lookup"><span data-stu-id="fc525-107">Constraint enforcing the file extension is acceptable for a given setting</span></span>


<span data-ttu-id="fc525-108">继承自[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="fc525-108">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="fc525-109">属性</span><span class="sxs-lookup"><span data-stu-id="fc525-109">Properties</span></span>
|<span data-ttu-id="fc525-110">属性</span><span class="sxs-lookup"><span data-stu-id="fc525-110">Property</span></span>|<span data-ttu-id="fc525-111">类型</span><span class="sxs-lookup"><span data-stu-id="fc525-111">Type</span></span>|<span data-ttu-id="fc525-112">说明</span><span class="sxs-lookup"><span data-stu-id="fc525-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc525-113">supportedExtensions</span><span class="sxs-lookup"><span data-stu-id="fc525-113">supportedExtensions</span></span>|<span data-ttu-id="fc525-114">String 集合</span><span class="sxs-lookup"><span data-stu-id="fc525-114">String collection</span></span>|<span data-ttu-id="fc525-115">为此设置上载可接受的文件扩展名</span><span class="sxs-lookup"><span data-stu-id="fc525-115">Acceptable file extensions to upload for this setting</span></span>|

## <a name="relationships"></a><span data-ttu-id="fc525-116">关系</span><span class="sxs-lookup"><span data-stu-id="fc525-116">Relationships</span></span>
<span data-ttu-id="fc525-117">无</span><span class="sxs-lookup"><span data-stu-id="fc525-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fc525-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fc525-118">JSON Representation</span></span>
<span data-ttu-id="fc525-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fc525-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettingFileConstraint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingFileConstraint",
  "supportedExtensions": [
    "String"
  ]
}
```



