---
title: iosWebContentFilterSpecificWebsitesAccess 资源类型
description: 表示 iOS Web 内容筛选器设置类型，该类型将 URL 书签安装到 iOS 内置浏览器中。 在课堂中，教师希望学生通过在其 iOS 设备上配置的浏览器书签来导航网站，而不能访问其他网站，这是一个示例方案。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f4129ce4f4332c78e5af6170b5ce48ab7aa19cee
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529812"
---
# <a name="ioswebcontentfilterspecificwebsitesaccess-resource-type"></a><span data-ttu-id="3eb29-104">iosWebContentFilterSpecificWebsitesAccess 资源类型</span><span class="sxs-lookup"><span data-stu-id="3eb29-104">iosWebContentFilterSpecificWebsitesAccess resource type</span></span>

<span data-ttu-id="3eb29-105">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="3eb29-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3eb29-106">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3eb29-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3eb29-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3eb29-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3eb29-108">表示 iOS Web 内容筛选器设置类型，该类型将 URL 书签安装到 iOS 内置浏览器中。</span><span class="sxs-lookup"><span data-stu-id="3eb29-108">Represents an iOS Web Content Filter setting type, which installs URL bookmarks into iOS built-in browser.</span></span> <span data-ttu-id="3eb29-109">在课堂中，教师希望学生通过在其 iOS 设备上配置的浏览器书签来导航网站，而不能访问其他网站，这是一个示例方案。</span><span class="sxs-lookup"><span data-stu-id="3eb29-109">An example scenario is in the classroom where teachers would like the students to navigate websites through browser bookmarks configured on their iOS devices, and no access to other sites.</span></span>


<span data-ttu-id="3eb29-110">继承自[iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)</span><span class="sxs-lookup"><span data-stu-id="3eb29-110">Inherits from [iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3eb29-111">属性</span><span class="sxs-lookup"><span data-stu-id="3eb29-111">Properties</span></span>
|<span data-ttu-id="3eb29-112">属性</span><span class="sxs-lookup"><span data-stu-id="3eb29-112">Property</span></span>|<span data-ttu-id="3eb29-113">类型</span><span class="sxs-lookup"><span data-stu-id="3eb29-113">Type</span></span>|<span data-ttu-id="3eb29-114">说明</span><span class="sxs-lookup"><span data-stu-id="3eb29-114">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3eb29-115">specificWebsitesOnly</span><span class="sxs-lookup"><span data-stu-id="3eb29-115">specificWebsitesOnly</span></span>|<span data-ttu-id="3eb29-116">[iosBookmark](../resources/intune-deviceconfig-iosbookmark.md)集合</span><span class="sxs-lookup"><span data-stu-id="3eb29-116">[iosBookmark](../resources/intune-deviceconfig-iosbookmark.md) collection</span></span>|<span data-ttu-id="3eb29-117">将安装到内置浏览器和用户的 URL 书签仅允许通过书签访问网站。</span><span class="sxs-lookup"><span data-stu-id="3eb29-117">URL bookmarks which will be installed into built-in browser and user is only allowed to access websites through bookmarks.</span></span> <span data-ttu-id="3eb29-118">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="3eb29-118">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="3eb29-119">websiteList</span><span class="sxs-lookup"><span data-stu-id="3eb29-119">websiteList</span></span>|<span data-ttu-id="3eb29-120">[iosBookmark](../resources/intune-deviceconfig-iosbookmark.md)集合</span><span class="sxs-lookup"><span data-stu-id="3eb29-120">[iosBookmark](../resources/intune-deviceconfig-iosbookmark.md) collection</span></span>|<span data-ttu-id="3eb29-121">将安装到内置浏览器和用户的 URL 书签仅允许通过书签访问网站。</span><span class="sxs-lookup"><span data-stu-id="3eb29-121">URL bookmarks which will be installed into built-in browser and user is only allowed to access websites through bookmarks.</span></span> <span data-ttu-id="3eb29-122">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="3eb29-122">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3eb29-123">关系</span><span class="sxs-lookup"><span data-stu-id="3eb29-123">Relationships</span></span>
<span data-ttu-id="3eb29-124">无</span><span class="sxs-lookup"><span data-stu-id="3eb29-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3eb29-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3eb29-125">JSON Representation</span></span>
<span data-ttu-id="3eb29-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3eb29-126">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosWebContentFilterSpecificWebsitesAccess"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosWebContentFilterSpecificWebsitesAccess",
  "specificWebsitesOnly": [
    {
      "@odata.type": "microsoft.graph.iosBookmark",
      "url": "String",
      "bookmarkFolder": "String",
      "displayName": "String"
    }
  ],
  "websiteList": [
    {
      "@odata.type": "microsoft.graph.iosBookmark",
      "url": "String",
      "bookmarkFolder": "String",
      "displayName": "String"
    }
  ]
}
```



