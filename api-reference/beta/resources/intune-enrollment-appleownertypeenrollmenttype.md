---
title: appleOwnerTypeEnrollmentType 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b48d6cf07131b02193180bafafdca59529fd6c4b
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43419509"
---
# <a name="appleownertypeenrollmenttype-resource-type"></a><span data-ttu-id="ff0a2-103">appleOwnerTypeEnrollmentType 资源类型</span><span class="sxs-lookup"><span data-stu-id="ff0a2-103">appleOwnerTypeEnrollmentType resource type</span></span>

<span data-ttu-id="ff0a2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff0a2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ff0a2-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ff0a2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ff0a2-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ff0a2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ff0a2-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="ff0a2-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="ff0a2-108">属性</span><span class="sxs-lookup"><span data-stu-id="ff0a2-108">Properties</span></span>
|<span data-ttu-id="ff0a2-109">属性</span><span class="sxs-lookup"><span data-stu-id="ff0a2-109">Property</span></span>|<span data-ttu-id="ff0a2-110">类型</span><span class="sxs-lookup"><span data-stu-id="ff0a2-110">Type</span></span>|<span data-ttu-id="ff0a2-111">说明</span><span class="sxs-lookup"><span data-stu-id="ff0a2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff0a2-112">所有者</span><span class="sxs-lookup"><span data-stu-id="ff0a2-112">ownerType</span></span>|[<span data-ttu-id="ff0a2-113">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="ff0a2-113">managedDeviceOwnerType</span></span>](../resources/intune-shared-manageddeviceownertype.md)|<span data-ttu-id="ff0a2-114">所有者类型。</span><span class="sxs-lookup"><span data-stu-id="ff0a2-114">The owner type.</span></span> <span data-ttu-id="ff0a2-115">可取值为：`unknown`、`company`、`personal`。</span><span class="sxs-lookup"><span data-stu-id="ff0a2-115">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="ff0a2-116">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="ff0a2-116">enrollmentType</span></span>|[<span data-ttu-id="ff0a2-117">appleUserInitiatedEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="ff0a2-117">appleUserInitiatedEnrollmentType</span></span>](../resources/intune-enrollment-appleuserinitiatedenrollmenttype.md)|<span data-ttu-id="ff0a2-118">注册类型。</span><span class="sxs-lookup"><span data-stu-id="ff0a2-118">The enrollment type.</span></span> <span data-ttu-id="ff0a2-119">可取值为：`unknown`、`device`、`user`。</span><span class="sxs-lookup"><span data-stu-id="ff0a2-119">Possible values are: `unknown`, `device`, `user`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ff0a2-120">关系</span><span class="sxs-lookup"><span data-stu-id="ff0a2-120">Relationships</span></span>
<span data-ttu-id="ff0a2-121">无</span><span class="sxs-lookup"><span data-stu-id="ff0a2-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ff0a2-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ff0a2-122">JSON Representation</span></span>
<span data-ttu-id="ff0a2-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ff0a2-123">Here is a JSON representation of the resource.</span></span>
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



