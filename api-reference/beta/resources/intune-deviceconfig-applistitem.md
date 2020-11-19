---
title: appListItem 资源类型
description: 表示托管应用程序列表中的应用
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b32e08474296894e2bb54135f6daab347b6fb7fa
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49260808"
---
# <a name="applistitem-resource-type"></a><span data-ttu-id="01281-103">appListItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="01281-103">appListItem resource type</span></span>

<span data-ttu-id="01281-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="01281-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="01281-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="01281-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="01281-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="01281-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="01281-107">表示托管应用程序列表中的应用</span><span class="sxs-lookup"><span data-stu-id="01281-107">Represents an app in the list of managed applications</span></span>

## <a name="properties"></a><span data-ttu-id="01281-108">属性</span><span class="sxs-lookup"><span data-stu-id="01281-108">Properties</span></span>
|<span data-ttu-id="01281-109">属性</span><span class="sxs-lookup"><span data-stu-id="01281-109">Property</span></span>|<span data-ttu-id="01281-110">类型</span><span class="sxs-lookup"><span data-stu-id="01281-110">Type</span></span>|<span data-ttu-id="01281-111">描述</span><span class="sxs-lookup"><span data-stu-id="01281-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="01281-112">name</span><span class="sxs-lookup"><span data-stu-id="01281-112">name</span></span>|<span data-ttu-id="01281-113">String</span><span class="sxs-lookup"><span data-stu-id="01281-113">String</span></span>|<span data-ttu-id="01281-114">应用程序名称</span><span class="sxs-lookup"><span data-stu-id="01281-114">The application name</span></span>|
|<span data-ttu-id="01281-115">publisher</span><span class="sxs-lookup"><span data-stu-id="01281-115">publisher</span></span>|<span data-ttu-id="01281-116">String</span><span class="sxs-lookup"><span data-stu-id="01281-116">String</span></span>|<span data-ttu-id="01281-117">应用程序发布者</span><span class="sxs-lookup"><span data-stu-id="01281-117">The publisher of the application</span></span>|
|<span data-ttu-id="01281-118">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="01281-118">appStoreUrl</span></span>|<span data-ttu-id="01281-119">String</span><span class="sxs-lookup"><span data-stu-id="01281-119">String</span></span>|<span data-ttu-id="01281-120">应用程序的应用商店 URL</span><span class="sxs-lookup"><span data-stu-id="01281-120">The Store URL of the application</span></span>|
|<span data-ttu-id="01281-121">appId</span><span class="sxs-lookup"><span data-stu-id="01281-121">appId</span></span>|<span data-ttu-id="01281-122">String</span><span class="sxs-lookup"><span data-stu-id="01281-122">String</span></span>|<span data-ttu-id="01281-123">应用程序或应用程序的捆绑标识符</span><span class="sxs-lookup"><span data-stu-id="01281-123">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="01281-124">关系</span><span class="sxs-lookup"><span data-stu-id="01281-124">Relationships</span></span>
<span data-ttu-id="01281-125">无</span><span class="sxs-lookup"><span data-stu-id="01281-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="01281-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="01281-126">JSON Representation</span></span>
<span data-ttu-id="01281-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="01281-127">Here is a JSON representation of the resource.</span></span>
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




