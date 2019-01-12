---
title: resourceAction 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 17d8bd52996ca9b129292c204dd498fcc5a65ac6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27963239"
---
# <a name="resourceaction-resource-type"></a><span data-ttu-id="d0c14-103">resourceAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="d0c14-103">resourceAction resource type</span></span>

> <span data-ttu-id="d0c14-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d0c14-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d0c14-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d0c14-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d0c14-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="d0c14-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d0c14-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d0c14-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="d0c14-108">属性</span><span class="sxs-lookup"><span data-stu-id="d0c14-108">Properties</span></span>
|<span data-ttu-id="d0c14-109">属性</span><span class="sxs-lookup"><span data-stu-id="d0c14-109">Property</span></span>|<span data-ttu-id="d0c14-110">类型</span><span class="sxs-lookup"><span data-stu-id="d0c14-110">Type</span></span>|<span data-ttu-id="d0c14-111">说明</span><span class="sxs-lookup"><span data-stu-id="d0c14-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d0c14-112">allowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="d0c14-112">allowedResourceActions</span></span>|<span data-ttu-id="d0c14-113">字符串集合</span><span class="sxs-lookup"><span data-stu-id="d0c14-113">String collection</span></span>|<span data-ttu-id="d0c14-114">允许的操作</span><span class="sxs-lookup"><span data-stu-id="d0c14-114">Allowed Actions</span></span>|
|<span data-ttu-id="d0c14-115">notAllowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="d0c14-115">notAllowedResourceActions</span></span>|<span data-ttu-id="d0c14-116">字符串集合</span><span class="sxs-lookup"><span data-stu-id="d0c14-116">String collection</span></span>|<span data-ttu-id="d0c14-117">不允许的操作</span><span class="sxs-lookup"><span data-stu-id="d0c14-117">Not Allowed Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="d0c14-118">关系</span><span class="sxs-lookup"><span data-stu-id="d0c14-118">Relationships</span></span>
<span data-ttu-id="d0c14-119">无</span><span class="sxs-lookup"><span data-stu-id="d0c14-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d0c14-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d0c14-120">JSON Representation</span></span>
<span data-ttu-id="d0c14-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d0c14-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.resourceAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.resourceAction",
  "allowedResourceActions": [
    "String"
  ],
  "notAllowedResourceActions": [
    "String"
  ]
}
```





