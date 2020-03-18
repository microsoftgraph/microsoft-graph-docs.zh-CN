---
title: deviceManagementSettingFileConstraint 资源类型
description: 强制实施文件扩展名的约束可接受给定设置
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9a9e5a3f4ce8cec54dbdd0f1a690b039b2da0524
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42785321"
---
# <a name="devicemanagementsettingfileconstraint-resource-type"></a><span data-ttu-id="097db-103">deviceManagementSettingFileConstraint 资源类型</span><span class="sxs-lookup"><span data-stu-id="097db-103">deviceManagementSettingFileConstraint resource type</span></span>

> <span data-ttu-id="097db-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="097db-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="097db-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="097db-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="097db-106">强制实施文件扩展名的约束可接受给定设置</span><span class="sxs-lookup"><span data-stu-id="097db-106">Constraint enforcing the file extension is acceptable for a given setting</span></span>


<span data-ttu-id="097db-107">继承自[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="097db-107">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="097db-108">属性</span><span class="sxs-lookup"><span data-stu-id="097db-108">Properties</span></span>
|<span data-ttu-id="097db-109">属性</span><span class="sxs-lookup"><span data-stu-id="097db-109">Property</span></span>|<span data-ttu-id="097db-110">类型</span><span class="sxs-lookup"><span data-stu-id="097db-110">Type</span></span>|<span data-ttu-id="097db-111">说明</span><span class="sxs-lookup"><span data-stu-id="097db-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="097db-112">supportedExtensions</span><span class="sxs-lookup"><span data-stu-id="097db-112">supportedExtensions</span></span>|<span data-ttu-id="097db-113">String collection</span><span class="sxs-lookup"><span data-stu-id="097db-113">String collection</span></span>|<span data-ttu-id="097db-114">为此设置上载可接受的文件扩展名</span><span class="sxs-lookup"><span data-stu-id="097db-114">Acceptable file extensions to upload for this setting</span></span>|

## <a name="relationships"></a><span data-ttu-id="097db-115">关系</span><span class="sxs-lookup"><span data-stu-id="097db-115">Relationships</span></span>
<span data-ttu-id="097db-116">无</span><span class="sxs-lookup"><span data-stu-id="097db-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="097db-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="097db-117">JSON Representation</span></span>
<span data-ttu-id="097db-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="097db-118">Here is a JSON representation of the resource.</span></span>
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



