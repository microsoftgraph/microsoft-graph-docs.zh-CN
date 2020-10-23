---
title: appleAppListItem 资源类型
description: 表示托管 Apple 应用程序列表中的应用程序
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 831991580d2b3d667011d84179a73957c6eeb200
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48703921"
---
# <a name="appleapplistitem-resource-type"></a><span data-ttu-id="5d60c-103">appleAppListItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="5d60c-103">appleAppListItem resource type</span></span>

<span data-ttu-id="5d60c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5d60c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5d60c-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5d60c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5d60c-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5d60c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5d60c-107">表示托管 Apple 应用程序列表中的应用程序</span><span class="sxs-lookup"><span data-stu-id="5d60c-107">Represents an app in the list of managed Apple applications</span></span>


<span data-ttu-id="5d60c-108">继承自 [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="5d60c-108">Inherits from [appListItem](../resources/intune-deviceconfig-applistitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="5d60c-109">属性</span><span class="sxs-lookup"><span data-stu-id="5d60c-109">Properties</span></span>
|<span data-ttu-id="5d60c-110">属性</span><span class="sxs-lookup"><span data-stu-id="5d60c-110">Property</span></span>|<span data-ttu-id="5d60c-111">类型</span><span class="sxs-lookup"><span data-stu-id="5d60c-111">Type</span></span>|<span data-ttu-id="5d60c-112">说明</span><span class="sxs-lookup"><span data-stu-id="5d60c-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5d60c-113">name</span><span class="sxs-lookup"><span data-stu-id="5d60c-113">name</span></span>|<span data-ttu-id="5d60c-114">String</span><span class="sxs-lookup"><span data-stu-id="5d60c-114">String</span></span>|<span data-ttu-id="5d60c-115">从[AppListItem](../resources/intune-deviceconfig-applistitem.md)继承的应用程序名称</span><span class="sxs-lookup"><span data-stu-id="5d60c-115">The application name Inherited from [appListItem](../resources/intune-deviceconfig-applistitem.md)</span></span>|
|<span data-ttu-id="5d60c-116">发布者</span><span class="sxs-lookup"><span data-stu-id="5d60c-116">publisher</span></span>|<span data-ttu-id="5d60c-117">String</span><span class="sxs-lookup"><span data-stu-id="5d60c-117">String</span></span>|<span data-ttu-id="5d60c-118">从[AppListItem](../resources/intune-deviceconfig-applistitem.md)继承的应用程序的发布者</span><span class="sxs-lookup"><span data-stu-id="5d60c-118">The publisher of the application Inherited from [appListItem](../resources/intune-deviceconfig-applistitem.md)</span></span>|
|<span data-ttu-id="5d60c-119">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="5d60c-119">appStoreUrl</span></span>|<span data-ttu-id="5d60c-120">String</span><span class="sxs-lookup"><span data-stu-id="5d60c-120">String</span></span>|<span data-ttu-id="5d60c-121">继承自[appListItem](../resources/intune-deviceconfig-applistitem.md)的应用程序的存储 URL</span><span class="sxs-lookup"><span data-stu-id="5d60c-121">The Store URL of the application Inherited from [appListItem](../resources/intune-deviceconfig-applistitem.md)</span></span>|
|<span data-ttu-id="5d60c-122">appId</span><span class="sxs-lookup"><span data-stu-id="5d60c-122">appId</span></span>|<span data-ttu-id="5d60c-123">String</span><span class="sxs-lookup"><span data-stu-id="5d60c-123">String</span></span>|<span data-ttu-id="5d60c-124">从[AppListItem](../resources/intune-deviceconfig-applistitem.md)继承的应用程序的应用程序或捆绑包标识符</span><span class="sxs-lookup"><span data-stu-id="5d60c-124">The application or bundle identifier of the application Inherited from [appListItem](../resources/intune-deviceconfig-applistitem.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="5d60c-125">关系</span><span class="sxs-lookup"><span data-stu-id="5d60c-125">Relationships</span></span>
<span data-ttu-id="5d60c-126">无</span><span class="sxs-lookup"><span data-stu-id="5d60c-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5d60c-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5d60c-127">JSON Representation</span></span>
<span data-ttu-id="5d60c-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5d60c-128">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appleAppListItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appleAppListItem",
  "name": "String",
  "publisher": "String",
  "appStoreUrl": "String",
  "appId": "String"
}
```





