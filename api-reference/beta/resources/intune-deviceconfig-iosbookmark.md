---
title: iosBookmark 资源类型
description: iOS URL 书签
ms.openlocfilehash: e2349e0d280c9798a03363ab90d378ff206c57bf
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043751"
---
# <a name="iosbookmark-resource-type"></a><span data-ttu-id="fdf72-103">iosBookmark 资源类型</span><span class="sxs-lookup"><span data-stu-id="fdf72-103">iosBookmark resource type</span></span>

> <span data-ttu-id="fdf72-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="fdf72-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fdf72-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="fdf72-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fdf72-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="fdf72-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fdf72-107">iOS URL 书签</span><span class="sxs-lookup"><span data-stu-id="fdf72-107">iOS URL bookmark</span></span>
## <a name="properties"></a><span data-ttu-id="fdf72-108">属性</span><span class="sxs-lookup"><span data-stu-id="fdf72-108">Properties</span></span>
|<span data-ttu-id="fdf72-109">属性</span><span class="sxs-lookup"><span data-stu-id="fdf72-109">Property</span></span>|<span data-ttu-id="fdf72-110">类型</span><span class="sxs-lookup"><span data-stu-id="fdf72-110">Type</span></span>|<span data-ttu-id="fdf72-111">说明</span><span class="sxs-lookup"><span data-stu-id="fdf72-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fdf72-112">url</span><span class="sxs-lookup"><span data-stu-id="fdf72-112">url</span></span>|<span data-ttu-id="fdf72-113">String</span><span class="sxs-lookup"><span data-stu-id="fdf72-113">String</span></span>|<span data-ttu-id="fdf72-114">允许访问的 URL</span><span class="sxs-lookup"><span data-stu-id="fdf72-114">URL allowed to access</span></span>|
|<span data-ttu-id="fdf72-115">bookmarkFolder</span><span class="sxs-lookup"><span data-stu-id="fdf72-115">bookmarkFolder</span></span>|<span data-ttu-id="fdf72-116">字符串</span><span class="sxs-lookup"><span data-stu-id="fdf72-116">String</span></span>|<span data-ttu-id="fdf72-117">向其中应在 Safari 中添加书签的文件夹</span><span class="sxs-lookup"><span data-stu-id="fdf72-117">The folder into which the bookmark should be added in Safari</span></span>|
|<span data-ttu-id="fdf72-118">displayName</span><span class="sxs-lookup"><span data-stu-id="fdf72-118">displayName</span></span>|<span data-ttu-id="fdf72-119">字符串</span><span class="sxs-lookup"><span data-stu-id="fdf72-119">String</span></span>|<span data-ttu-id="fdf72-120">书签的显示名称</span><span class="sxs-lookup"><span data-stu-id="fdf72-120">The display name of the bookmark</span></span>|

## <a name="relationships"></a><span data-ttu-id="fdf72-121">Relationships</span><span class="sxs-lookup"><span data-stu-id="fdf72-121">Relationships</span></span>
<span data-ttu-id="fdf72-122">无</span><span class="sxs-lookup"><span data-stu-id="fdf72-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="fdf72-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fdf72-123">JSON Representation</span></span>
<span data-ttu-id="fdf72-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fdf72-124">Here is a JSON representation of the resource.</span></span>
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





