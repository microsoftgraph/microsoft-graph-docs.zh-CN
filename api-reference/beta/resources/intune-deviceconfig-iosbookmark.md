---
title: iosBookmark 资源类型
description: iOS URL 书签
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9d2f96b872d09eaf3c954f18a31219d6bfe17ddb
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34988361"
---
# <a name="iosbookmark-resource-type"></a><span data-ttu-id="e73eb-103">iosBookmark 资源类型</span><span class="sxs-lookup"><span data-stu-id="e73eb-103">iosBookmark resource type</span></span>

> <span data-ttu-id="e73eb-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e73eb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e73eb-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e73eb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e73eb-106">iOS URL 书签</span><span class="sxs-lookup"><span data-stu-id="e73eb-106">iOS URL bookmark</span></span>

## <a name="properties"></a><span data-ttu-id="e73eb-107">属性</span><span class="sxs-lookup"><span data-stu-id="e73eb-107">Properties</span></span>
|<span data-ttu-id="e73eb-108">属性</span><span class="sxs-lookup"><span data-stu-id="e73eb-108">Property</span></span>|<span data-ttu-id="e73eb-109">类型</span><span class="sxs-lookup"><span data-stu-id="e73eb-109">Type</span></span>|<span data-ttu-id="e73eb-110">说明</span><span class="sxs-lookup"><span data-stu-id="e73eb-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e73eb-111">url</span><span class="sxs-lookup"><span data-stu-id="e73eb-111">url</span></span>|<span data-ttu-id="e73eb-112">String</span><span class="sxs-lookup"><span data-stu-id="e73eb-112">String</span></span>|<span data-ttu-id="e73eb-113">允许访问的 URL</span><span class="sxs-lookup"><span data-stu-id="e73eb-113">URL allowed to access</span></span>|
|<span data-ttu-id="e73eb-114">bookmarkFolder</span><span class="sxs-lookup"><span data-stu-id="e73eb-114">bookmarkFolder</span></span>|<span data-ttu-id="e73eb-115">String</span><span class="sxs-lookup"><span data-stu-id="e73eb-115">String</span></span>|<span data-ttu-id="e73eb-116">应在 Safari 中添加书签的文件夹</span><span class="sxs-lookup"><span data-stu-id="e73eb-116">The folder into which the bookmark should be added in Safari</span></span>|
|<span data-ttu-id="e73eb-117">displayName</span><span class="sxs-lookup"><span data-stu-id="e73eb-117">displayName</span></span>|<span data-ttu-id="e73eb-118">String</span><span class="sxs-lookup"><span data-stu-id="e73eb-118">String</span></span>|<span data-ttu-id="e73eb-119">书签的显示名称</span><span class="sxs-lookup"><span data-stu-id="e73eb-119">The display name of the bookmark</span></span>|

## <a name="relationships"></a><span data-ttu-id="e73eb-120">关系</span><span class="sxs-lookup"><span data-stu-id="e73eb-120">Relationships</span></span>
<span data-ttu-id="e73eb-121">无</span><span class="sxs-lookup"><span data-stu-id="e73eb-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e73eb-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e73eb-122">JSON Representation</span></span>
<span data-ttu-id="e73eb-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e73eb-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosBookmark"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosBookmark",
  "url": "String",
  "bookmarkFolder": "String",
  "displayName": "String"
}
```





