---
title: iosBookmark 资源类型
description: iOS URL 书签
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 769afaef5370cd55c8edc30a057a9bba15893d88
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48031660"
---
# <a name="iosbookmark-resource-type"></a><span data-ttu-id="fab4b-103">iosBookmark 资源类型</span><span class="sxs-lookup"><span data-stu-id="fab4b-103">iosBookmark resource type</span></span>

<span data-ttu-id="fab4b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fab4b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fab4b-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="fab4b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fab4b-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fab4b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fab4b-107">iOS URL 书签</span><span class="sxs-lookup"><span data-stu-id="fab4b-107">iOS URL bookmark</span></span>

## <a name="properties"></a><span data-ttu-id="fab4b-108">属性</span><span class="sxs-lookup"><span data-stu-id="fab4b-108">Properties</span></span>
|<span data-ttu-id="fab4b-109">属性</span><span class="sxs-lookup"><span data-stu-id="fab4b-109">Property</span></span>|<span data-ttu-id="fab4b-110">类型</span><span class="sxs-lookup"><span data-stu-id="fab4b-110">Type</span></span>|<span data-ttu-id="fab4b-111">说明</span><span class="sxs-lookup"><span data-stu-id="fab4b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fab4b-112">url</span><span class="sxs-lookup"><span data-stu-id="fab4b-112">url</span></span>|<span data-ttu-id="fab4b-113">String</span><span class="sxs-lookup"><span data-stu-id="fab4b-113">String</span></span>|<span data-ttu-id="fab4b-114">允许访问的 URL</span><span class="sxs-lookup"><span data-stu-id="fab4b-114">URL allowed to access</span></span>|
|<span data-ttu-id="fab4b-115">bookmarkFolder</span><span class="sxs-lookup"><span data-stu-id="fab4b-115">bookmarkFolder</span></span>|<span data-ttu-id="fab4b-116">String</span><span class="sxs-lookup"><span data-stu-id="fab4b-116">String</span></span>|<span data-ttu-id="fab4b-117">应在 Safari 中添加书签的文件夹</span><span class="sxs-lookup"><span data-stu-id="fab4b-117">The folder into which the bookmark should be added in Safari</span></span>|
|<span data-ttu-id="fab4b-118">displayName</span><span class="sxs-lookup"><span data-stu-id="fab4b-118">displayName</span></span>|<span data-ttu-id="fab4b-119">String</span><span class="sxs-lookup"><span data-stu-id="fab4b-119">String</span></span>|<span data-ttu-id="fab4b-120">书签的显示名称</span><span class="sxs-lookup"><span data-stu-id="fab4b-120">The display name of the bookmark</span></span>|

## <a name="relationships"></a><span data-ttu-id="fab4b-121">关系</span><span class="sxs-lookup"><span data-stu-id="fab4b-121">Relationships</span></span>
<span data-ttu-id="fab4b-122">无</span><span class="sxs-lookup"><span data-stu-id="fab4b-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fab4b-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fab4b-123">JSON Representation</span></span>
<span data-ttu-id="fab4b-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fab4b-124">Here is a JSON representation of the resource.</span></span>
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






