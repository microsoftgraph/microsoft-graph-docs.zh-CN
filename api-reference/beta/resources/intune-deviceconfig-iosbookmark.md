---
title: iosBookmark 资源类型
description: iOS URL 书签
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e95f3bfd40bdf5ca5782aa9233a020623d32d6a5
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395907"
---
# <a name="iosbookmark-resource-type"></a><span data-ttu-id="b0ae9-103">iosBookmark 资源类型</span><span class="sxs-lookup"><span data-stu-id="b0ae9-103">iosBookmark resource type</span></span>

> <span data-ttu-id="b0ae9-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="b0ae9-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b0ae9-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b0ae9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b0ae9-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b0ae9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b0ae9-107">iOS URL 书签</span><span class="sxs-lookup"><span data-stu-id="b0ae9-107">iOS URL bookmark</span></span>

## <a name="properties"></a><span data-ttu-id="b0ae9-108">属性</span><span class="sxs-lookup"><span data-stu-id="b0ae9-108">Properties</span></span>
|<span data-ttu-id="b0ae9-109">属性</span><span class="sxs-lookup"><span data-stu-id="b0ae9-109">Property</span></span>|<span data-ttu-id="b0ae9-110">类型</span><span class="sxs-lookup"><span data-stu-id="b0ae9-110">Type</span></span>|<span data-ttu-id="b0ae9-111">说明</span><span class="sxs-lookup"><span data-stu-id="b0ae9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0ae9-112">url</span><span class="sxs-lookup"><span data-stu-id="b0ae9-112">url</span></span>|<span data-ttu-id="b0ae9-113">String</span><span class="sxs-lookup"><span data-stu-id="b0ae9-113">String</span></span>|<span data-ttu-id="b0ae9-114">允许访问的 URL</span><span class="sxs-lookup"><span data-stu-id="b0ae9-114">URL allowed to access</span></span>|
|<span data-ttu-id="b0ae9-115">bookmarkFolder</span><span class="sxs-lookup"><span data-stu-id="b0ae9-115">bookmarkFolder</span></span>|<span data-ttu-id="b0ae9-116">String</span><span class="sxs-lookup"><span data-stu-id="b0ae9-116">String</span></span>|<span data-ttu-id="b0ae9-117">向其中应在 Safari 中添加书签的文件夹</span><span class="sxs-lookup"><span data-stu-id="b0ae9-117">The folder into which the bookmark should be added in Safari</span></span>|
|<span data-ttu-id="b0ae9-118">displayName</span><span class="sxs-lookup"><span data-stu-id="b0ae9-118">displayName</span></span>|<span data-ttu-id="b0ae9-119">String</span><span class="sxs-lookup"><span data-stu-id="b0ae9-119">String</span></span>|<span data-ttu-id="b0ae9-120">书签的显示名称</span><span class="sxs-lookup"><span data-stu-id="b0ae9-120">The display name of the bookmark</span></span>|

## <a name="relationships"></a><span data-ttu-id="b0ae9-121">关系</span><span class="sxs-lookup"><span data-stu-id="b0ae9-121">Relationships</span></span>
<span data-ttu-id="b0ae9-122">无</span><span class="sxs-lookup"><span data-stu-id="b0ae9-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b0ae9-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b0ae9-123">JSON Representation</span></span>
<span data-ttu-id="b0ae9-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b0ae9-124">Here is a JSON representation of the resource.</span></span>
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




