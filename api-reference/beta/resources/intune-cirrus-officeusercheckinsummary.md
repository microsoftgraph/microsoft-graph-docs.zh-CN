---
title: officeUserCheckinSummary 资源类型
description: 描述租户签入统计信息的实体。
localization_priority: Normal
author: dougeby
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8564f7d0d2fb06218b141b7e9369f2096bdec982
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43462517"
---
# <a name="officeusercheckinsummary-resource-type"></a><span data-ttu-id="567d9-103">officeUserCheckinSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="567d9-103">officeUserCheckinSummary resource type</span></span>

<span data-ttu-id="567d9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="567d9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="567d9-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="567d9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="567d9-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="567d9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="567d9-107">描述租户签入统计信息的实体。</span><span class="sxs-lookup"><span data-stu-id="567d9-107">Entity that describes  tenant check-in stats.</span></span>

## <a name="properties"></a><span data-ttu-id="567d9-108">属性</span><span class="sxs-lookup"><span data-stu-id="567d9-108">Properties</span></span>
|<span data-ttu-id="567d9-109">属性</span><span class="sxs-lookup"><span data-stu-id="567d9-109">Property</span></span>|<span data-ttu-id="567d9-110">类型</span><span class="sxs-lookup"><span data-stu-id="567d9-110">Type</span></span>|<span data-ttu-id="567d9-111">说明</span><span class="sxs-lookup"><span data-stu-id="567d9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="567d9-112">succeededUserCount</span><span class="sxs-lookup"><span data-stu-id="567d9-112">succeededUserCount</span></span>|<span data-ttu-id="567d9-113">Int32</span><span class="sxs-lookup"><span data-stu-id="567d9-113">Int32</span></span>|<span data-ttu-id="567d9-114">最近3个月内成功的用户签入次数总计。</span><span class="sxs-lookup"><span data-stu-id="567d9-114">Total successful user check ins for the last 3 months.</span></span>|
|<span data-ttu-id="567d9-115">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="567d9-115">failedUserCount</span></span>|<span data-ttu-id="567d9-116">Int32</span><span class="sxs-lookup"><span data-stu-id="567d9-116">Int32</span></span>|<span data-ttu-id="567d9-117">最近3个月的用户签入失败总计。</span><span class="sxs-lookup"><span data-stu-id="567d9-117">Total failed user check ins for the last 3 months.</span></span>|

## <a name="relationships"></a><span data-ttu-id="567d9-118">关系</span><span class="sxs-lookup"><span data-stu-id="567d9-118">Relationships</span></span>
<span data-ttu-id="567d9-119">无</span><span class="sxs-lookup"><span data-stu-id="567d9-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="567d9-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="567d9-120">JSON Representation</span></span>
<span data-ttu-id="567d9-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="567d9-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.officeUserCheckinSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.officeUserCheckinSummary",
  "succeededUserCount": 1024,
  "failedUserCount": 1024
}
```



