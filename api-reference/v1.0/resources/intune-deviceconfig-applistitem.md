---
title: appListItem 资源类型
description: 表示托管应用程序列表中的应用
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 5b9aa0a35767078b7c91f72b7a8b06a450cc9f33
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028607"
---
# <a name="applistitem-resource-type"></a><span data-ttu-id="f2b15-103">appListItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="f2b15-103">appListItem resource type</span></span>

> <span data-ttu-id="f2b15-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f2b15-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f2b15-105">表示托管应用程序列表中的应用</span><span class="sxs-lookup"><span data-stu-id="f2b15-105">Represents an app in the list of managed applications</span></span>

## <a name="properties"></a><span data-ttu-id="f2b15-106">属性</span><span class="sxs-lookup"><span data-stu-id="f2b15-106">Properties</span></span>
|<span data-ttu-id="f2b15-107">属性</span><span class="sxs-lookup"><span data-stu-id="f2b15-107">Property</span></span>|<span data-ttu-id="f2b15-108">类型</span><span class="sxs-lookup"><span data-stu-id="f2b15-108">Type</span></span>|<span data-ttu-id="f2b15-109">说明</span><span class="sxs-lookup"><span data-stu-id="f2b15-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f2b15-110">name</span><span class="sxs-lookup"><span data-stu-id="f2b15-110">name</span></span>|<span data-ttu-id="f2b15-111">字符串</span><span class="sxs-lookup"><span data-stu-id="f2b15-111">String</span></span>|<span data-ttu-id="f2b15-112">应用程序名称</span><span class="sxs-lookup"><span data-stu-id="f2b15-112">The application name</span></span>|
|<span data-ttu-id="f2b15-113">publisher</span><span class="sxs-lookup"><span data-stu-id="f2b15-113">publisher</span></span>|<span data-ttu-id="f2b15-114">String</span><span class="sxs-lookup"><span data-stu-id="f2b15-114">String</span></span>|<span data-ttu-id="f2b15-115">应用程序发布者</span><span class="sxs-lookup"><span data-stu-id="f2b15-115">The publisher of the application</span></span>|
|<span data-ttu-id="f2b15-116">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="f2b15-116">appStoreUrl</span></span>|<span data-ttu-id="f2b15-117">String</span><span class="sxs-lookup"><span data-stu-id="f2b15-117">String</span></span>|<span data-ttu-id="f2b15-118">应用程序的应用商店 URL</span><span class="sxs-lookup"><span data-stu-id="f2b15-118">The Store URL of the application</span></span>|
|<span data-ttu-id="f2b15-119">appId</span><span class="sxs-lookup"><span data-stu-id="f2b15-119">appId</span></span>|<span data-ttu-id="f2b15-120">String</span><span class="sxs-lookup"><span data-stu-id="f2b15-120">String</span></span>|<span data-ttu-id="f2b15-121">应用程序或应用程序的捆绑标识符</span><span class="sxs-lookup"><span data-stu-id="f2b15-121">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="f2b15-122">关系</span><span class="sxs-lookup"><span data-stu-id="f2b15-122">Relationships</span></span>
<span data-ttu-id="f2b15-123">无</span><span class="sxs-lookup"><span data-stu-id="f2b15-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f2b15-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f2b15-124">JSON Representation</span></span>
<span data-ttu-id="f2b15-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f2b15-125">Here is a JSON representation of the resource.</span></span>
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



