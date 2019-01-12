---
title: appListItem 资源类型
description: 表示托管应用程序列表中的应用
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 492828fdef95815704083ec8f496e38a10dc3559
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27923332"
---
# <a name="applistitem-resource-type"></a><span data-ttu-id="64b5f-103">appListItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="64b5f-103">appListItem resource type</span></span>

> <span data-ttu-id="64b5f-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="64b5f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="64b5f-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="64b5f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="64b5f-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="64b5f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="64b5f-107">表示托管应用程序列表中的应用</span><span class="sxs-lookup"><span data-stu-id="64b5f-107">Represents an app in the list of managed applications</span></span>
## <a name="properties"></a><span data-ttu-id="64b5f-108">属性</span><span class="sxs-lookup"><span data-stu-id="64b5f-108">Properties</span></span>
|<span data-ttu-id="64b5f-109">属性</span><span class="sxs-lookup"><span data-stu-id="64b5f-109">Property</span></span>|<span data-ttu-id="64b5f-110">类型</span><span class="sxs-lookup"><span data-stu-id="64b5f-110">Type</span></span>|<span data-ttu-id="64b5f-111">说明</span><span class="sxs-lookup"><span data-stu-id="64b5f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="64b5f-112">name</span><span class="sxs-lookup"><span data-stu-id="64b5f-112">name</span></span>|<span data-ttu-id="64b5f-113">String</span><span class="sxs-lookup"><span data-stu-id="64b5f-113">String</span></span>|<span data-ttu-id="64b5f-114">应用程序名称</span><span class="sxs-lookup"><span data-stu-id="64b5f-114">The application name</span></span>|
|<span data-ttu-id="64b5f-115">publisher</span><span class="sxs-lookup"><span data-stu-id="64b5f-115">publisher</span></span>|<span data-ttu-id="64b5f-116">String</span><span class="sxs-lookup"><span data-stu-id="64b5f-116">String</span></span>|<span data-ttu-id="64b5f-117">应用程序发布者</span><span class="sxs-lookup"><span data-stu-id="64b5f-117">The publisher of the application</span></span>|
|<span data-ttu-id="64b5f-118">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="64b5f-118">appStoreUrl</span></span>|<span data-ttu-id="64b5f-119">String</span><span class="sxs-lookup"><span data-stu-id="64b5f-119">String</span></span>|<span data-ttu-id="64b5f-120">应用程序的应用商店 URL</span><span class="sxs-lookup"><span data-stu-id="64b5f-120">The Store URL of the application</span></span>|
|<span data-ttu-id="64b5f-121">appId</span><span class="sxs-lookup"><span data-stu-id="64b5f-121">appId</span></span>|<span data-ttu-id="64b5f-122">String</span><span class="sxs-lookup"><span data-stu-id="64b5f-122">String</span></span>|<span data-ttu-id="64b5f-123">应用程序或应用程序的捆绑标识符</span><span class="sxs-lookup"><span data-stu-id="64b5f-123">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="64b5f-124">关系</span><span class="sxs-lookup"><span data-stu-id="64b5f-124">Relationships</span></span>
<span data-ttu-id="64b5f-125">无</span><span class="sxs-lookup"><span data-stu-id="64b5f-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="64b5f-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="64b5f-126">JSON Representation</span></span>
<span data-ttu-id="64b5f-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="64b5f-127">Here is a JSON representation of the resource.</span></span>
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





