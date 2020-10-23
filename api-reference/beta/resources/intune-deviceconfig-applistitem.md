---
title: appListItem 资源类型
description: 表示托管应用程序列表中的应用
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ccf980b0874ea40989eb297abd6bbf455e827f95
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48708828"
---
# <a name="applistitem-resource-type"></a><span data-ttu-id="e1321-103">appListItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="e1321-103">appListItem resource type</span></span>

<span data-ttu-id="e1321-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e1321-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e1321-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e1321-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e1321-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e1321-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e1321-107">表示托管应用程序列表中的应用</span><span class="sxs-lookup"><span data-stu-id="e1321-107">Represents an app in the list of managed applications</span></span>

## <a name="properties"></a><span data-ttu-id="e1321-108">属性</span><span class="sxs-lookup"><span data-stu-id="e1321-108">Properties</span></span>
|<span data-ttu-id="e1321-109">属性</span><span class="sxs-lookup"><span data-stu-id="e1321-109">Property</span></span>|<span data-ttu-id="e1321-110">类型</span><span class="sxs-lookup"><span data-stu-id="e1321-110">Type</span></span>|<span data-ttu-id="e1321-111">说明</span><span class="sxs-lookup"><span data-stu-id="e1321-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1321-112">name</span><span class="sxs-lookup"><span data-stu-id="e1321-112">name</span></span>|<span data-ttu-id="e1321-113">String</span><span class="sxs-lookup"><span data-stu-id="e1321-113">String</span></span>|<span data-ttu-id="e1321-114">应用程序名称</span><span class="sxs-lookup"><span data-stu-id="e1321-114">The application name</span></span>|
|<span data-ttu-id="e1321-115">publisher</span><span class="sxs-lookup"><span data-stu-id="e1321-115">publisher</span></span>|<span data-ttu-id="e1321-116">String</span><span class="sxs-lookup"><span data-stu-id="e1321-116">String</span></span>|<span data-ttu-id="e1321-117">应用程序发布者</span><span class="sxs-lookup"><span data-stu-id="e1321-117">The publisher of the application</span></span>|
|<span data-ttu-id="e1321-118">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="e1321-118">appStoreUrl</span></span>|<span data-ttu-id="e1321-119">String</span><span class="sxs-lookup"><span data-stu-id="e1321-119">String</span></span>|<span data-ttu-id="e1321-120">应用程序的应用商店 URL</span><span class="sxs-lookup"><span data-stu-id="e1321-120">The Store URL of the application</span></span>|
|<span data-ttu-id="e1321-121">appId</span><span class="sxs-lookup"><span data-stu-id="e1321-121">appId</span></span>|<span data-ttu-id="e1321-122">String</span><span class="sxs-lookup"><span data-stu-id="e1321-122">String</span></span>|<span data-ttu-id="e1321-123">应用程序或应用程序的捆绑标识符</span><span class="sxs-lookup"><span data-stu-id="e1321-123">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="e1321-124">关系</span><span class="sxs-lookup"><span data-stu-id="e1321-124">Relationships</span></span>
<span data-ttu-id="e1321-125">无</span><span class="sxs-lookup"><span data-stu-id="e1321-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e1321-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e1321-126">JSON Representation</span></span>
<span data-ttu-id="e1321-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e1321-127">Here is a JSON representation of the resource.</span></span>
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





