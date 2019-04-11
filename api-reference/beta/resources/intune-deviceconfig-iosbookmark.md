---
title: iosBookmark 资源类型
description: iOS URL 书签
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5231ccbae496e310e414c6429190e0b4d53cbaa7
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31782798"
---
# <a name="iosbookmark-resource-type"></a><span data-ttu-id="88867-103">iosBookmark 资源类型</span><span class="sxs-lookup"><span data-stu-id="88867-103">iosBookmark resource type</span></span>

> <span data-ttu-id="88867-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="88867-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="88867-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="88867-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="88867-106">iOS URL 书签</span><span class="sxs-lookup"><span data-stu-id="88867-106">iOS URL bookmark</span></span>

## <a name="properties"></a><span data-ttu-id="88867-107">属性</span><span class="sxs-lookup"><span data-stu-id="88867-107">Properties</span></span>
|<span data-ttu-id="88867-108">属性</span><span class="sxs-lookup"><span data-stu-id="88867-108">Property</span></span>|<span data-ttu-id="88867-109">类型</span><span class="sxs-lookup"><span data-stu-id="88867-109">Type</span></span>|<span data-ttu-id="88867-110">说明</span><span class="sxs-lookup"><span data-stu-id="88867-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88867-111">url</span><span class="sxs-lookup"><span data-stu-id="88867-111">url</span></span>|<span data-ttu-id="88867-112">String</span><span class="sxs-lookup"><span data-stu-id="88867-112">String</span></span>|<span data-ttu-id="88867-113">允许访问的 URL</span><span class="sxs-lookup"><span data-stu-id="88867-113">URL allowed to access</span></span>|
|<span data-ttu-id="88867-114">bookmarkFolder</span><span class="sxs-lookup"><span data-stu-id="88867-114">bookmarkFolder</span></span>|<span data-ttu-id="88867-115">String</span><span class="sxs-lookup"><span data-stu-id="88867-115">String</span></span>|<span data-ttu-id="88867-116">应在 Safari 中添加书签的文件夹</span><span class="sxs-lookup"><span data-stu-id="88867-116">The folder into which the bookmark should be added in Safari</span></span>|
|<span data-ttu-id="88867-117">displayName</span><span class="sxs-lookup"><span data-stu-id="88867-117">displayName</span></span>|<span data-ttu-id="88867-118">String</span><span class="sxs-lookup"><span data-stu-id="88867-118">String</span></span>|<span data-ttu-id="88867-119">书签的显示名称</span><span class="sxs-lookup"><span data-stu-id="88867-119">The display name of the bookmark</span></span>|

## <a name="relationships"></a><span data-ttu-id="88867-120">关系</span><span class="sxs-lookup"><span data-stu-id="88867-120">Relationships</span></span>
<span data-ttu-id="88867-121">无</span><span class="sxs-lookup"><span data-stu-id="88867-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="88867-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="88867-122">JSON Representation</span></span>
<span data-ttu-id="88867-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="88867-123">Here is a JSON representation of the resource.</span></span>
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





