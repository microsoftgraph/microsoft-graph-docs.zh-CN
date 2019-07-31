---
title: appListItem 资源类型
description: 表示托管应用程序列表中的应用
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8f985994ae3d69280ac1bd55626096cf6de46adf
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35971114"
---
# <a name="applistitem-resource-type"></a><span data-ttu-id="0313f-103">appListItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="0313f-103">appListItem resource type</span></span>

> <span data-ttu-id="0313f-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0313f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0313f-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0313f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0313f-106">表示托管应用程序列表中的应用</span><span class="sxs-lookup"><span data-stu-id="0313f-106">Represents an app in the list of managed applications</span></span>

## <a name="properties"></a><span data-ttu-id="0313f-107">属性</span><span class="sxs-lookup"><span data-stu-id="0313f-107">Properties</span></span>
|<span data-ttu-id="0313f-108">属性</span><span class="sxs-lookup"><span data-stu-id="0313f-108">Property</span></span>|<span data-ttu-id="0313f-109">类型</span><span class="sxs-lookup"><span data-stu-id="0313f-109">Type</span></span>|<span data-ttu-id="0313f-110">说明</span><span class="sxs-lookup"><span data-stu-id="0313f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0313f-111">name</span><span class="sxs-lookup"><span data-stu-id="0313f-111">name</span></span>|<span data-ttu-id="0313f-112">字符串</span><span class="sxs-lookup"><span data-stu-id="0313f-112">String</span></span>|<span data-ttu-id="0313f-113">应用程序名称</span><span class="sxs-lookup"><span data-stu-id="0313f-113">The application name</span></span>|
|<span data-ttu-id="0313f-114">publisher</span><span class="sxs-lookup"><span data-stu-id="0313f-114">publisher</span></span>|<span data-ttu-id="0313f-115">String</span><span class="sxs-lookup"><span data-stu-id="0313f-115">String</span></span>|<span data-ttu-id="0313f-116">应用程序发布者</span><span class="sxs-lookup"><span data-stu-id="0313f-116">The publisher of the application</span></span>|
|<span data-ttu-id="0313f-117">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="0313f-117">appStoreUrl</span></span>|<span data-ttu-id="0313f-118">String</span><span class="sxs-lookup"><span data-stu-id="0313f-118">String</span></span>|<span data-ttu-id="0313f-119">应用程序的应用商店 URL</span><span class="sxs-lookup"><span data-stu-id="0313f-119">The Store URL of the application</span></span>|
|<span data-ttu-id="0313f-120">appId</span><span class="sxs-lookup"><span data-stu-id="0313f-120">appId</span></span>|<span data-ttu-id="0313f-121">String</span><span class="sxs-lookup"><span data-stu-id="0313f-121">String</span></span>|<span data-ttu-id="0313f-122">应用程序或应用程序的捆绑标识符</span><span class="sxs-lookup"><span data-stu-id="0313f-122">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="0313f-123">关系</span><span class="sxs-lookup"><span data-stu-id="0313f-123">Relationships</span></span>
<span data-ttu-id="0313f-124">无</span><span class="sxs-lookup"><span data-stu-id="0313f-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0313f-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0313f-125">JSON Representation</span></span>
<span data-ttu-id="0313f-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0313f-126">Here is a JSON representation of the resource.</span></span>
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





