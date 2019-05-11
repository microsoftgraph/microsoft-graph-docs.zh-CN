---
title: appListItem 资源类型
description: 表示托管应用程序列表中的应用
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d29fca9155ac14c7b8ebf9ad862bda3bed874353
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33947713"
---
# <a name="applistitem-resource-type"></a><span data-ttu-id="4b84d-103">appListItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="4b84d-103">appListItem resource type</span></span>

> <span data-ttu-id="4b84d-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4b84d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4b84d-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4b84d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4b84d-106">表示托管应用程序列表中的应用</span><span class="sxs-lookup"><span data-stu-id="4b84d-106">Represents an app in the list of managed applications</span></span>

## <a name="properties"></a><span data-ttu-id="4b84d-107">属性</span><span class="sxs-lookup"><span data-stu-id="4b84d-107">Properties</span></span>
|<span data-ttu-id="4b84d-108">属性</span><span class="sxs-lookup"><span data-stu-id="4b84d-108">Property</span></span>|<span data-ttu-id="4b84d-109">类型</span><span class="sxs-lookup"><span data-stu-id="4b84d-109">Type</span></span>|<span data-ttu-id="4b84d-110">说明</span><span class="sxs-lookup"><span data-stu-id="4b84d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b84d-111">name</span><span class="sxs-lookup"><span data-stu-id="4b84d-111">name</span></span>|<span data-ttu-id="4b84d-112">字符串</span><span class="sxs-lookup"><span data-stu-id="4b84d-112">String</span></span>|<span data-ttu-id="4b84d-113">应用程序名称</span><span class="sxs-lookup"><span data-stu-id="4b84d-113">The application name</span></span>|
|<span data-ttu-id="4b84d-114">publisher</span><span class="sxs-lookup"><span data-stu-id="4b84d-114">publisher</span></span>|<span data-ttu-id="4b84d-115">String</span><span class="sxs-lookup"><span data-stu-id="4b84d-115">String</span></span>|<span data-ttu-id="4b84d-116">应用程序发布者</span><span class="sxs-lookup"><span data-stu-id="4b84d-116">The publisher of the application</span></span>|
|<span data-ttu-id="4b84d-117">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="4b84d-117">appStoreUrl</span></span>|<span data-ttu-id="4b84d-118">String</span><span class="sxs-lookup"><span data-stu-id="4b84d-118">String</span></span>|<span data-ttu-id="4b84d-119">应用程序的应用商店 URL</span><span class="sxs-lookup"><span data-stu-id="4b84d-119">The Store URL of the application</span></span>|
|<span data-ttu-id="4b84d-120">appId</span><span class="sxs-lookup"><span data-stu-id="4b84d-120">appId</span></span>|<span data-ttu-id="4b84d-121">String</span><span class="sxs-lookup"><span data-stu-id="4b84d-121">String</span></span>|<span data-ttu-id="4b84d-122">应用程序或应用程序的捆绑标识符</span><span class="sxs-lookup"><span data-stu-id="4b84d-122">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="4b84d-123">关系</span><span class="sxs-lookup"><span data-stu-id="4b84d-123">Relationships</span></span>
<span data-ttu-id="4b84d-124">无</span><span class="sxs-lookup"><span data-stu-id="4b84d-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4b84d-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4b84d-125">JSON Representation</span></span>
<span data-ttu-id="4b84d-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4b84d-126">Here is a JSON representation of the resource.</span></span>
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




