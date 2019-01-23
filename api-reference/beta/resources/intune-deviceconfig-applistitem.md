---
title: appListItem 资源类型
description: 表示托管应用程序列表中的应用
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 9571b622fc098f384f7c3a6c62b1d1e10d89f663
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29405413"
---
# <a name="applistitem-resource-type"></a><span data-ttu-id="61cc1-103">appListItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="61cc1-103">appListItem resource type</span></span>

> <span data-ttu-id="61cc1-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="61cc1-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="61cc1-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="61cc1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="61cc1-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="61cc1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="61cc1-107">表示托管应用程序列表中的应用</span><span class="sxs-lookup"><span data-stu-id="61cc1-107">Represents an app in the list of managed applications</span></span>

## <a name="properties"></a><span data-ttu-id="61cc1-108">属性</span><span class="sxs-lookup"><span data-stu-id="61cc1-108">Properties</span></span>
|<span data-ttu-id="61cc1-109">属性</span><span class="sxs-lookup"><span data-stu-id="61cc1-109">Property</span></span>|<span data-ttu-id="61cc1-110">类型</span><span class="sxs-lookup"><span data-stu-id="61cc1-110">Type</span></span>|<span data-ttu-id="61cc1-111">说明</span><span class="sxs-lookup"><span data-stu-id="61cc1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="61cc1-112">name</span><span class="sxs-lookup"><span data-stu-id="61cc1-112">name</span></span>|<span data-ttu-id="61cc1-113">String</span><span class="sxs-lookup"><span data-stu-id="61cc1-113">String</span></span>|<span data-ttu-id="61cc1-114">应用程序名称</span><span class="sxs-lookup"><span data-stu-id="61cc1-114">The application name</span></span>|
|<span data-ttu-id="61cc1-115">publisher</span><span class="sxs-lookup"><span data-stu-id="61cc1-115">publisher</span></span>|<span data-ttu-id="61cc1-116">String</span><span class="sxs-lookup"><span data-stu-id="61cc1-116">String</span></span>|<span data-ttu-id="61cc1-117">应用程序发布者</span><span class="sxs-lookup"><span data-stu-id="61cc1-117">The publisher of the application</span></span>|
|<span data-ttu-id="61cc1-118">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="61cc1-118">appStoreUrl</span></span>|<span data-ttu-id="61cc1-119">String</span><span class="sxs-lookup"><span data-stu-id="61cc1-119">String</span></span>|<span data-ttu-id="61cc1-120">应用程序的应用商店 URL</span><span class="sxs-lookup"><span data-stu-id="61cc1-120">The Store URL of the application</span></span>|
|<span data-ttu-id="61cc1-121">appId</span><span class="sxs-lookup"><span data-stu-id="61cc1-121">appId</span></span>|<span data-ttu-id="61cc1-122">String</span><span class="sxs-lookup"><span data-stu-id="61cc1-122">String</span></span>|<span data-ttu-id="61cc1-123">应用程序或应用程序的捆绑标识符</span><span class="sxs-lookup"><span data-stu-id="61cc1-123">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="61cc1-124">关系</span><span class="sxs-lookup"><span data-stu-id="61cc1-124">Relationships</span></span>
<span data-ttu-id="61cc1-125">无</span><span class="sxs-lookup"><span data-stu-id="61cc1-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="61cc1-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="61cc1-126">JSON Representation</span></span>
<span data-ttu-id="61cc1-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="61cc1-127">Here is a JSON representation of the resource.</span></span>
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




