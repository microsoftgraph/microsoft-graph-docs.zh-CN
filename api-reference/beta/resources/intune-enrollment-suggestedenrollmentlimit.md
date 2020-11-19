---
title: suggestedEnrollmentLimit 资源类型
description: 当给定注册类型时，suggestedEnrollmentLimit 资源表示建议的注册限制。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 880fb5d77c7fa16a23349918973a33ba0952e07a
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49256258"
---
# <a name="suggestedenrollmentlimit-resource-type"></a><span data-ttu-id="ff412-103">suggestedEnrollmentLimit 资源类型</span><span class="sxs-lookup"><span data-stu-id="ff412-103">suggestedEnrollmentLimit resource type</span></span>

<span data-ttu-id="ff412-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff412-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ff412-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ff412-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ff412-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ff412-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ff412-107">当给定注册类型时，suggestedEnrollmentLimit 资源表示建议的注册限制。</span><span class="sxs-lookup"><span data-stu-id="ff412-107">The suggestedEnrollmentLimit resource represents the suggested enrollment limit when given an enrollment type.</span></span>

## <a name="properties"></a><span data-ttu-id="ff412-108">属性</span><span class="sxs-lookup"><span data-stu-id="ff412-108">Properties</span></span>
|<span data-ttu-id="ff412-109">属性</span><span class="sxs-lookup"><span data-stu-id="ff412-109">Property</span></span>|<span data-ttu-id="ff412-110">类型</span><span class="sxs-lookup"><span data-stu-id="ff412-110">Type</span></span>|<span data-ttu-id="ff412-111">描述</span><span class="sxs-lookup"><span data-stu-id="ff412-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff412-112">suggestedDailyLimit</span><span class="sxs-lookup"><span data-stu-id="ff412-112">suggestedDailyLimit</span></span>|<span data-ttu-id="ff412-113">Int32</span><span class="sxs-lookup"><span data-stu-id="ff412-113">Int32</span></span>|<span data-ttu-id="ff412-114">一天内建议的登记限制</span><span class="sxs-lookup"><span data-stu-id="ff412-114">The suggested enrollment limit within a day</span></span>|

## <a name="relationships"></a><span data-ttu-id="ff412-115">关系</span><span class="sxs-lookup"><span data-stu-id="ff412-115">Relationships</span></span>
<span data-ttu-id="ff412-116">无</span><span class="sxs-lookup"><span data-stu-id="ff412-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ff412-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ff412-117">JSON Representation</span></span>
<span data-ttu-id="ff412-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ff412-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.suggestedEnrollmentLimit"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.suggestedEnrollmentLimit",
  "suggestedDailyLimit": 1024
}
```




