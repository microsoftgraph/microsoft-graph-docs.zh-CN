---
title: officeUserCheckinSummary 资源类型
description: 描述租户签入统计信息的实体。
localization_priority: Normal
author: rolyon
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f3daa7fd8691fe6c6894a2305e9f5c1533f597b5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42488066"
---
# <a name="officeusercheckinsummary-resource-type"></a><span data-ttu-id="db5d7-103">officeUserCheckinSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="db5d7-103">officeUserCheckinSummary resource type</span></span>

<span data-ttu-id="db5d7-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="db5d7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="db5d7-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="db5d7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="db5d7-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="db5d7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="db5d7-107">描述租户签入统计信息的实体。</span><span class="sxs-lookup"><span data-stu-id="db5d7-107">Entity that describes  tenant check-in stats.</span></span>

## <a name="properties"></a><span data-ttu-id="db5d7-108">属性</span><span class="sxs-lookup"><span data-stu-id="db5d7-108">Properties</span></span>
|<span data-ttu-id="db5d7-109">属性</span><span class="sxs-lookup"><span data-stu-id="db5d7-109">Property</span></span>|<span data-ttu-id="db5d7-110">类型</span><span class="sxs-lookup"><span data-stu-id="db5d7-110">Type</span></span>|<span data-ttu-id="db5d7-111">说明</span><span class="sxs-lookup"><span data-stu-id="db5d7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="db5d7-112">succeededUserCount</span><span class="sxs-lookup"><span data-stu-id="db5d7-112">succeededUserCount</span></span>|<span data-ttu-id="db5d7-113">Int32</span><span class="sxs-lookup"><span data-stu-id="db5d7-113">Int32</span></span>|<span data-ttu-id="db5d7-114">最近3个月内成功的用户签入次数总计。</span><span class="sxs-lookup"><span data-stu-id="db5d7-114">Total successful user check ins for the last 3 months.</span></span>|
|<span data-ttu-id="db5d7-115">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="db5d7-115">failedUserCount</span></span>|<span data-ttu-id="db5d7-116">Int32</span><span class="sxs-lookup"><span data-stu-id="db5d7-116">Int32</span></span>|<span data-ttu-id="db5d7-117">最近3个月的用户签入失败总计。</span><span class="sxs-lookup"><span data-stu-id="db5d7-117">Total failed user check ins for the last 3 months.</span></span>|

## <a name="relationships"></a><span data-ttu-id="db5d7-118">关系</span><span class="sxs-lookup"><span data-stu-id="db5d7-118">Relationships</span></span>
<span data-ttu-id="db5d7-119">无</span><span class="sxs-lookup"><span data-stu-id="db5d7-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="db5d7-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="db5d7-120">JSON Representation</span></span>
<span data-ttu-id="db5d7-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="db5d7-121">Here is a JSON representation of the resource.</span></span>
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



