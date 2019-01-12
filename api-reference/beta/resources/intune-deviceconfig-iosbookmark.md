---
title: iosBookmark 资源类型
description: iOS URL 书签
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: cbf39a2eee5064b7d3ddfa474b1f70758d4c7047
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938172"
---
# <a name="iosbookmark-resource-type"></a><span data-ttu-id="e2a90-103">iosBookmark 资源类型</span><span class="sxs-lookup"><span data-stu-id="e2a90-103">iosBookmark resource type</span></span>

> <span data-ttu-id="e2a90-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="e2a90-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e2a90-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e2a90-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e2a90-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="e2a90-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e2a90-107">iOS URL 书签</span><span class="sxs-lookup"><span data-stu-id="e2a90-107">iOS URL bookmark</span></span>
## <a name="properties"></a><span data-ttu-id="e2a90-108">属性</span><span class="sxs-lookup"><span data-stu-id="e2a90-108">Properties</span></span>
|<span data-ttu-id="e2a90-109">属性</span><span class="sxs-lookup"><span data-stu-id="e2a90-109">Property</span></span>|<span data-ttu-id="e2a90-110">类型</span><span class="sxs-lookup"><span data-stu-id="e2a90-110">Type</span></span>|<span data-ttu-id="e2a90-111">说明</span><span class="sxs-lookup"><span data-stu-id="e2a90-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2a90-112">url</span><span class="sxs-lookup"><span data-stu-id="e2a90-112">url</span></span>|<span data-ttu-id="e2a90-113">String</span><span class="sxs-lookup"><span data-stu-id="e2a90-113">String</span></span>|<span data-ttu-id="e2a90-114">允许访问的 URL</span><span class="sxs-lookup"><span data-stu-id="e2a90-114">URL allowed to access</span></span>|
|<span data-ttu-id="e2a90-115">bookmarkFolder</span><span class="sxs-lookup"><span data-stu-id="e2a90-115">bookmarkFolder</span></span>|<span data-ttu-id="e2a90-116">字符串</span><span class="sxs-lookup"><span data-stu-id="e2a90-116">String</span></span>|<span data-ttu-id="e2a90-117">向其中应在 Safari 中添加书签的文件夹</span><span class="sxs-lookup"><span data-stu-id="e2a90-117">The folder into which the bookmark should be added in Safari</span></span>|
|<span data-ttu-id="e2a90-118">displayName</span><span class="sxs-lookup"><span data-stu-id="e2a90-118">displayName</span></span>|<span data-ttu-id="e2a90-119">字符串</span><span class="sxs-lookup"><span data-stu-id="e2a90-119">String</span></span>|<span data-ttu-id="e2a90-120">书签的显示名称</span><span class="sxs-lookup"><span data-stu-id="e2a90-120">The display name of the bookmark</span></span>|

## <a name="relationships"></a><span data-ttu-id="e2a90-121">Relationships</span><span class="sxs-lookup"><span data-stu-id="e2a90-121">Relationships</span></span>
<span data-ttu-id="e2a90-122">无</span><span class="sxs-lookup"><span data-stu-id="e2a90-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e2a90-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e2a90-123">JSON Representation</span></span>
<span data-ttu-id="e2a90-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e2a90-124">Here is a JSON representation of the resource.</span></span>
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





