---
title: appleOwnerTypeEnrollmentType 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5d86dc53b6fb65125dbcba32854769f71634d7fa
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49207545"
---
# <a name="appleownertypeenrollmenttype-resource-type"></a><span data-ttu-id="236f9-103">appleOwnerTypeEnrollmentType 资源类型</span><span class="sxs-lookup"><span data-stu-id="236f9-103">appleOwnerTypeEnrollmentType resource type</span></span>

<span data-ttu-id="236f9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="236f9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="236f9-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="236f9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="236f9-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="236f9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="236f9-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="236f9-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="236f9-108">属性</span><span class="sxs-lookup"><span data-stu-id="236f9-108">Properties</span></span>
|<span data-ttu-id="236f9-109">属性</span><span class="sxs-lookup"><span data-stu-id="236f9-109">Property</span></span>|<span data-ttu-id="236f9-110">类型</span><span class="sxs-lookup"><span data-stu-id="236f9-110">Type</span></span>|<span data-ttu-id="236f9-111">说明</span><span class="sxs-lookup"><span data-stu-id="236f9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="236f9-112">所有者</span><span class="sxs-lookup"><span data-stu-id="236f9-112">ownerType</span></span>|[<span data-ttu-id="236f9-113">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="236f9-113">managedDeviceOwnerType</span></span>](../resources/intune-shared-manageddeviceownertype.md)|<span data-ttu-id="236f9-114">所有者类型。</span><span class="sxs-lookup"><span data-stu-id="236f9-114">The owner type.</span></span> <span data-ttu-id="236f9-115">可取值为：`unknown`、`company`、`personal`。</span><span class="sxs-lookup"><span data-stu-id="236f9-115">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="236f9-116">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="236f9-116">enrollmentType</span></span>|[<span data-ttu-id="236f9-117">appleUserInitiatedEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="236f9-117">appleUserInitiatedEnrollmentType</span></span>](../resources/intune-enrollment-appleuserinitiatedenrollmenttype.md)|<span data-ttu-id="236f9-118">注册类型。</span><span class="sxs-lookup"><span data-stu-id="236f9-118">The enrollment type.</span></span> <span data-ttu-id="236f9-119">可取值为：`unknown`、`device`、`user`。</span><span class="sxs-lookup"><span data-stu-id="236f9-119">Possible values are: `unknown`, `device`, `user`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="236f9-120">关系</span><span class="sxs-lookup"><span data-stu-id="236f9-120">Relationships</span></span>
<span data-ttu-id="236f9-121">无</span><span class="sxs-lookup"><span data-stu-id="236f9-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="236f9-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="236f9-122">JSON Representation</span></span>
<span data-ttu-id="236f9-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="236f9-123">Here is a JSON representation of the resource.</span></span>
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




