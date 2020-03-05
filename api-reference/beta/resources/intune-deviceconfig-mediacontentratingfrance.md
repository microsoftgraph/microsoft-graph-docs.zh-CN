---
title: mediaContentRatingFrance 资源类型
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 078cdc458514344472aca5731b56f05bec3849dd
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529628"
---
# <a name="mediacontentratingfrance-resource-type"></a><span data-ttu-id="62831-103">mediaContentRatingFrance 资源类型</span><span class="sxs-lookup"><span data-stu-id="62831-103">mediaContentRatingFrance resource type</span></span>

<span data-ttu-id="62831-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="62831-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="62831-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="62831-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="62831-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="62831-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="62831-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="62831-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="62831-108">属性</span><span class="sxs-lookup"><span data-stu-id="62831-108">Properties</span></span>
|<span data-ttu-id="62831-109">属性</span><span class="sxs-lookup"><span data-stu-id="62831-109">Property</span></span>|<span data-ttu-id="62831-110">类型</span><span class="sxs-lookup"><span data-stu-id="62831-110">Type</span></span>|<span data-ttu-id="62831-111">说明</span><span class="sxs-lookup"><span data-stu-id="62831-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="62831-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="62831-112">movieRating</span></span>|[<span data-ttu-id="62831-113">ratingFranceMoviesType</span><span class="sxs-lookup"><span data-stu-id="62831-113">ratingFranceMoviesType</span></span>](../resources/intune-deviceconfig-ratingfrancemoviestype.md)|<span data-ttu-id="62831-114">为法国选择的电影评级。</span><span class="sxs-lookup"><span data-stu-id="62831-114">Movies rating selected for France.</span></span> <span data-ttu-id="62831-115">可取值为：`allAllowed`、`allBlocked`、`agesAbove10`、`agesAbove12`、`agesAbove16`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="62831-115">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|
|<span data-ttu-id="62831-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="62831-116">tvRating</span></span>|[<span data-ttu-id="62831-117">ratingFranceTelevisionType</span><span class="sxs-lookup"><span data-stu-id="62831-117">ratingFranceTelevisionType</span></span>](../resources/intune-deviceconfig-ratingfrancetelevisiontype.md)|<span data-ttu-id="62831-118">为法国选择的电视评级。</span><span class="sxs-lookup"><span data-stu-id="62831-118">TV rating selected for France.</span></span> <span data-ttu-id="62831-119">可取值为：`allAllowed`、`allBlocked`、`agesAbove10`、`agesAbove12`、`agesAbove16`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="62831-119">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="62831-120">关系</span><span class="sxs-lookup"><span data-stu-id="62831-120">Relationships</span></span>
<span data-ttu-id="62831-121">无</span><span class="sxs-lookup"><span data-stu-id="62831-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="62831-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="62831-122">JSON Representation</span></span>
<span data-ttu-id="62831-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="62831-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingFrance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingFrance",
  "movieRating": "String",
  "tvRating": "String"
}
```



