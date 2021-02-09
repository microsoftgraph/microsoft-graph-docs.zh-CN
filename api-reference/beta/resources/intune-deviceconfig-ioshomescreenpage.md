---
title: iosHomeScreenPage 资源类型
description: 主页上包含应用、文件夹和 Web 剪辑的页面。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 53385201015b7d22223e9d39f173416feb111b6c
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161801"
---
# <a name="ioshomescreenpage-resource-type"></a><span data-ttu-id="d5b6e-103">iosHomeScreenPage 资源类型</span><span class="sxs-lookup"><span data-stu-id="d5b6e-103">iosHomeScreenPage resource type</span></span>

<span data-ttu-id="d5b6e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d5b6e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d5b6e-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d5b6e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d5b6e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d5b6e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d5b6e-107">主页上包含应用、文件夹和 Web 剪辑的页面。</span><span class="sxs-lookup"><span data-stu-id="d5b6e-107">A page containing apps, folders, and web clips on the Home Screen.</span></span>

## <a name="properties"></a><span data-ttu-id="d5b6e-108">属性</span><span class="sxs-lookup"><span data-stu-id="d5b6e-108">Properties</span></span>
|<span data-ttu-id="d5b6e-109">属性</span><span class="sxs-lookup"><span data-stu-id="d5b6e-109">Property</span></span>|<span data-ttu-id="d5b6e-110">类型</span><span class="sxs-lookup"><span data-stu-id="d5b6e-110">Type</span></span>|<span data-ttu-id="d5b6e-111">说明</span><span class="sxs-lookup"><span data-stu-id="d5b6e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5b6e-112">displayName</span><span class="sxs-lookup"><span data-stu-id="d5b6e-112">displayName</span></span>|<span data-ttu-id="d5b6e-113">String</span><span class="sxs-lookup"><span data-stu-id="d5b6e-113">String</span></span>|<span data-ttu-id="d5b6e-114">页面的名称</span><span class="sxs-lookup"><span data-stu-id="d5b6e-114">Name of the page</span></span>|
|<span data-ttu-id="d5b6e-115">图标</span><span class="sxs-lookup"><span data-stu-id="d5b6e-115">icons</span></span>|<span data-ttu-id="d5b6e-116">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d5b6e-116">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="d5b6e-117">要显示在页面上的应用、文件夹和 Web 剪辑的列表。</span><span class="sxs-lookup"><span data-stu-id="d5b6e-117">A list of apps, folders, and web clips to appear on a page.</span></span> <span data-ttu-id="d5b6e-118">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="d5b6e-118">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d5b6e-119">关系</span><span class="sxs-lookup"><span data-stu-id="d5b6e-119">Relationships</span></span>
<span data-ttu-id="d5b6e-120">无</span><span class="sxs-lookup"><span data-stu-id="d5b6e-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d5b6e-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d5b6e-121">JSON Representation</span></span>
<span data-ttu-id="d5b6e-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d5b6e-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenPage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenPage",
  "displayName": "String",
  "icons": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenFolder",
      "displayName": "String",
      "pages": [
        {
          "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
          "displayName": "String",
          "apps": [
            {
              "@odata.type": "microsoft.graph.iosHomeScreenApp",
              "displayName": "String",
              "bundleID": "String",
              "isWebClip": true
            }
          ]
        }
      ]
    }
  ]
}
```




