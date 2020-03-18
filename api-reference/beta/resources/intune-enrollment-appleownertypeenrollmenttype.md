---
title: appleOwnerTypeEnrollmentType 资源类型
description: 尚未记录
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: fb4cb2787389e632fef73132f701010d0353aa0c
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42783576"
---
# <a name="appleownertypeenrollmenttype-resource-type"></a><span data-ttu-id="b6294-103">appleOwnerTypeEnrollmentType 资源类型</span><span class="sxs-lookup"><span data-stu-id="b6294-103">appleOwnerTypeEnrollmentType resource type</span></span>

> <span data-ttu-id="b6294-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b6294-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b6294-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b6294-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b6294-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="b6294-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="b6294-107">属性</span><span class="sxs-lookup"><span data-stu-id="b6294-107">Properties</span></span>
|<span data-ttu-id="b6294-108">属性</span><span class="sxs-lookup"><span data-stu-id="b6294-108">Property</span></span>|<span data-ttu-id="b6294-109">类型</span><span class="sxs-lookup"><span data-stu-id="b6294-109">Type</span></span>|<span data-ttu-id="b6294-110">说明</span><span class="sxs-lookup"><span data-stu-id="b6294-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b6294-111">所有者</span><span class="sxs-lookup"><span data-stu-id="b6294-111">ownerType</span></span>|[<span data-ttu-id="b6294-112">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="b6294-112">managedDeviceOwnerType</span></span>](../resources/intune-shared-manageddeviceownertype.md)|<span data-ttu-id="b6294-113">所有者类型。</span><span class="sxs-lookup"><span data-stu-id="b6294-113">The owner type.</span></span> <span data-ttu-id="b6294-114">可取值为：`unknown`、`company`、`personal`。</span><span class="sxs-lookup"><span data-stu-id="b6294-114">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="b6294-115">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="b6294-115">enrollmentType</span></span>|[<span data-ttu-id="b6294-116">appleUserInitiatedEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="b6294-116">appleUserInitiatedEnrollmentType</span></span>](../resources/intune-enrollment-appleuserinitiatedenrollmenttype.md)|<span data-ttu-id="b6294-117">注册类型。</span><span class="sxs-lookup"><span data-stu-id="b6294-117">The enrollment type.</span></span> <span data-ttu-id="b6294-118">可取值为：`unknown`、`device`、`user`。</span><span class="sxs-lookup"><span data-stu-id="b6294-118">Possible values are: `unknown`, `device`, `user`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b6294-119">关系</span><span class="sxs-lookup"><span data-stu-id="b6294-119">Relationships</span></span>
<span data-ttu-id="b6294-120">无</span><span class="sxs-lookup"><span data-stu-id="b6294-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b6294-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b6294-121">JSON Representation</span></span>
<span data-ttu-id="b6294-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b6294-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appleOwnerTypeEnrollmentType"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appleOwnerTypeEnrollmentType",
  "ownerType": "String",
  "enrollmentType": "String"
}
```



