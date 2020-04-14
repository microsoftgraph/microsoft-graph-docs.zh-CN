---
title: iosBookmark 资源类型
description: iOS URL 书签
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3789d905d285561e56b7a21664214f777987524e
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43444197"
---
# <a name="iosbookmark-resource-type"></a><span data-ttu-id="0e261-103">iosBookmark 资源类型</span><span class="sxs-lookup"><span data-stu-id="0e261-103">iosBookmark resource type</span></span>

<span data-ttu-id="0e261-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0e261-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0e261-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0e261-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0e261-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0e261-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0e261-107">iOS URL 书签</span><span class="sxs-lookup"><span data-stu-id="0e261-107">iOS URL bookmark</span></span>

## <a name="properties"></a><span data-ttu-id="0e261-108">属性</span><span class="sxs-lookup"><span data-stu-id="0e261-108">Properties</span></span>
|<span data-ttu-id="0e261-109">属性</span><span class="sxs-lookup"><span data-stu-id="0e261-109">Property</span></span>|<span data-ttu-id="0e261-110">类型</span><span class="sxs-lookup"><span data-stu-id="0e261-110">Type</span></span>|<span data-ttu-id="0e261-111">说明</span><span class="sxs-lookup"><span data-stu-id="0e261-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0e261-112">url</span><span class="sxs-lookup"><span data-stu-id="0e261-112">url</span></span>|<span data-ttu-id="0e261-113">String</span><span class="sxs-lookup"><span data-stu-id="0e261-113">String</span></span>|<span data-ttu-id="0e261-114">允许访问的 URL</span><span class="sxs-lookup"><span data-stu-id="0e261-114">URL allowed to access</span></span>|
|<span data-ttu-id="0e261-115">bookmarkFolder</span><span class="sxs-lookup"><span data-stu-id="0e261-115">bookmarkFolder</span></span>|<span data-ttu-id="0e261-116">String</span><span class="sxs-lookup"><span data-stu-id="0e261-116">String</span></span>|<span data-ttu-id="0e261-117">应在 Safari 中添加书签的文件夹</span><span class="sxs-lookup"><span data-stu-id="0e261-117">The folder into which the bookmark should be added in Safari</span></span>|
|<span data-ttu-id="0e261-118">displayName</span><span class="sxs-lookup"><span data-stu-id="0e261-118">displayName</span></span>|<span data-ttu-id="0e261-119">String</span><span class="sxs-lookup"><span data-stu-id="0e261-119">String</span></span>|<span data-ttu-id="0e261-120">书签的显示名称</span><span class="sxs-lookup"><span data-stu-id="0e261-120">The display name of the bookmark</span></span>|

## <a name="relationships"></a><span data-ttu-id="0e261-121">关系</span><span class="sxs-lookup"><span data-stu-id="0e261-121">Relationships</span></span>
<span data-ttu-id="0e261-122">无</span><span class="sxs-lookup"><span data-stu-id="0e261-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0e261-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0e261-123">JSON Representation</span></span>
<span data-ttu-id="0e261-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0e261-124">Here is a JSON representation of the resource.</span></span>
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



