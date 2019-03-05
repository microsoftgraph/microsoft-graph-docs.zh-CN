---
title: appListItem 资源类型
description: 表示托管应用程序列表中的应用
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: eb81c8edfae3f9b33be4636e9fd7f15fa758e789
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30253076"
---
# <a name="applistitem-resource-type"></a><span data-ttu-id="2ee5c-103">appListItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="2ee5c-103">appListItem resource type</span></span>

> <span data-ttu-id="2ee5c-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2ee5c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2ee5c-105">表示托管应用程序列表中的应用</span><span class="sxs-lookup"><span data-stu-id="2ee5c-105">Represents an app in the list of managed applications</span></span>

## <a name="properties"></a><span data-ttu-id="2ee5c-106">属性</span><span class="sxs-lookup"><span data-stu-id="2ee5c-106">Properties</span></span>
|<span data-ttu-id="2ee5c-107">属性</span><span class="sxs-lookup"><span data-stu-id="2ee5c-107">Property</span></span>|<span data-ttu-id="2ee5c-108">类型</span><span class="sxs-lookup"><span data-stu-id="2ee5c-108">Type</span></span>|<span data-ttu-id="2ee5c-109">说明</span><span class="sxs-lookup"><span data-stu-id="2ee5c-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ee5c-110">name</span><span class="sxs-lookup"><span data-stu-id="2ee5c-110">name</span></span>|<span data-ttu-id="2ee5c-111">String</span><span class="sxs-lookup"><span data-stu-id="2ee5c-111">String</span></span>|<span data-ttu-id="2ee5c-112">应用程序名称</span><span class="sxs-lookup"><span data-stu-id="2ee5c-112">The application name</span></span>|
|<span data-ttu-id="2ee5c-113">publisher</span><span class="sxs-lookup"><span data-stu-id="2ee5c-113">publisher</span></span>|<span data-ttu-id="2ee5c-114">String</span><span class="sxs-lookup"><span data-stu-id="2ee5c-114">String</span></span>|<span data-ttu-id="2ee5c-115">应用程序发布者</span><span class="sxs-lookup"><span data-stu-id="2ee5c-115">The publisher of the application</span></span>|
|<span data-ttu-id="2ee5c-116">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="2ee5c-116">appStoreUrl</span></span>|<span data-ttu-id="2ee5c-117">String</span><span class="sxs-lookup"><span data-stu-id="2ee5c-117">String</span></span>|<span data-ttu-id="2ee5c-118">应用程序的应用商店 URL</span><span class="sxs-lookup"><span data-stu-id="2ee5c-118">The Store URL of the application</span></span>|
|<span data-ttu-id="2ee5c-119">appId</span><span class="sxs-lookup"><span data-stu-id="2ee5c-119">appId</span></span>|<span data-ttu-id="2ee5c-120">String</span><span class="sxs-lookup"><span data-stu-id="2ee5c-120">String</span></span>|<span data-ttu-id="2ee5c-121">应用程序或应用程序的捆绑标识符</span><span class="sxs-lookup"><span data-stu-id="2ee5c-121">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="2ee5c-122">关系</span><span class="sxs-lookup"><span data-stu-id="2ee5c-122">Relationships</span></span>
<span data-ttu-id="2ee5c-123">无</span><span class="sxs-lookup"><span data-stu-id="2ee5c-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2ee5c-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2ee5c-124">JSON Representation</span></span>
<span data-ttu-id="2ee5c-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2ee5c-125">Here is a JSON representation of the resource.</span></span>
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



