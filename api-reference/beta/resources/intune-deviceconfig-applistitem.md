---
title: appListItem 资源类型
description: 表示托管应用程序列表中的应用
author: tfitzmac
ms.openlocfilehash: 825e88dd5bd32cadfd9a8bfa291ab67036c8180b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27343224"
---
# <a name="applistitem-resource-type"></a><span data-ttu-id="ecd02-103">appListItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="ecd02-103">appListItem resource type</span></span>

> <span data-ttu-id="ecd02-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ecd02-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ecd02-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ecd02-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ecd02-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="ecd02-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ecd02-107">表示托管应用程序列表中的应用</span><span class="sxs-lookup"><span data-stu-id="ecd02-107">Represents an app in the list of managed applications</span></span>
## <a name="properties"></a><span data-ttu-id="ecd02-108">属性</span><span class="sxs-lookup"><span data-stu-id="ecd02-108">Properties</span></span>
|<span data-ttu-id="ecd02-109">属性</span><span class="sxs-lookup"><span data-stu-id="ecd02-109">Property</span></span>|<span data-ttu-id="ecd02-110">类型</span><span class="sxs-lookup"><span data-stu-id="ecd02-110">Type</span></span>|<span data-ttu-id="ecd02-111">说明</span><span class="sxs-lookup"><span data-stu-id="ecd02-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ecd02-112">name</span><span class="sxs-lookup"><span data-stu-id="ecd02-112">name</span></span>|<span data-ttu-id="ecd02-113">String</span><span class="sxs-lookup"><span data-stu-id="ecd02-113">String</span></span>|<span data-ttu-id="ecd02-114">应用程序名称</span><span class="sxs-lookup"><span data-stu-id="ecd02-114">The application name</span></span>|
|<span data-ttu-id="ecd02-115">publisher</span><span class="sxs-lookup"><span data-stu-id="ecd02-115">publisher</span></span>|<span data-ttu-id="ecd02-116">String</span><span class="sxs-lookup"><span data-stu-id="ecd02-116">String</span></span>|<span data-ttu-id="ecd02-117">应用程序发布者</span><span class="sxs-lookup"><span data-stu-id="ecd02-117">The publisher of the application</span></span>|
|<span data-ttu-id="ecd02-118">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="ecd02-118">appStoreUrl</span></span>|<span data-ttu-id="ecd02-119">String</span><span class="sxs-lookup"><span data-stu-id="ecd02-119">String</span></span>|<span data-ttu-id="ecd02-120">应用程序的应用商店 URL</span><span class="sxs-lookup"><span data-stu-id="ecd02-120">The Store URL of the application</span></span>|
|<span data-ttu-id="ecd02-121">appId</span><span class="sxs-lookup"><span data-stu-id="ecd02-121">appId</span></span>|<span data-ttu-id="ecd02-122">String</span><span class="sxs-lookup"><span data-stu-id="ecd02-122">String</span></span>|<span data-ttu-id="ecd02-123">应用程序或应用程序的捆绑标识符</span><span class="sxs-lookup"><span data-stu-id="ecd02-123">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="ecd02-124">关系</span><span class="sxs-lookup"><span data-stu-id="ecd02-124">Relationships</span></span>
<span data-ttu-id="ecd02-125">无</span><span class="sxs-lookup"><span data-stu-id="ecd02-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ecd02-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ecd02-126">JSON Representation</span></span>
<span data-ttu-id="ecd02-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ecd02-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appListItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appListItem",
  "name": "String",
  "publisher": "String",
  "appStoreUrl": "String",
  "appId": "String"
}
```





