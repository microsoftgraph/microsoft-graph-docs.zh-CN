---
title: iosHomeScreenPage 资源类型
description: 主页上包含应用、文件夹和 Web 剪辑的页面。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9bc9880f63bc27ce4cdab44b128d6d373e348fb1
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760048"
---
# <a name="ioshomescreenpage-resource-type"></a><span data-ttu-id="23709-103">iosHomeScreenPage 资源类型</span><span class="sxs-lookup"><span data-stu-id="23709-103">iosHomeScreenPage resource type</span></span>

<span data-ttu-id="23709-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="23709-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="23709-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="23709-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="23709-106">主页上包含应用、文件夹和 Web 剪辑的页面。</span><span class="sxs-lookup"><span data-stu-id="23709-106">A page containing apps, folders, and web clips on the Home Screen.</span></span>

## <a name="properties"></a><span data-ttu-id="23709-107">属性</span><span class="sxs-lookup"><span data-stu-id="23709-107">Properties</span></span>
|<span data-ttu-id="23709-108">属性</span><span class="sxs-lookup"><span data-stu-id="23709-108">Property</span></span>|<span data-ttu-id="23709-109">类型</span><span class="sxs-lookup"><span data-stu-id="23709-109">Type</span></span>|<span data-ttu-id="23709-110">说明</span><span class="sxs-lookup"><span data-stu-id="23709-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23709-111">displayName</span><span class="sxs-lookup"><span data-stu-id="23709-111">displayName</span></span>|<span data-ttu-id="23709-112">String</span><span class="sxs-lookup"><span data-stu-id="23709-112">String</span></span>|<span data-ttu-id="23709-113">页面的名称</span><span class="sxs-lookup"><span data-stu-id="23709-113">Name of the page</span></span>|
|<span data-ttu-id="23709-114">图标</span><span class="sxs-lookup"><span data-stu-id="23709-114">icons</span></span>|<span data-ttu-id="23709-115">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="23709-115">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="23709-116">要显示在页面上的应用、文件夹和 Web 剪辑的列表。</span><span class="sxs-lookup"><span data-stu-id="23709-116">A list of apps, folders, and web clips to appear on a page.</span></span> <span data-ttu-id="23709-117">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="23709-117">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="23709-118">关系</span><span class="sxs-lookup"><span data-stu-id="23709-118">Relationships</span></span>
<span data-ttu-id="23709-119">无</span><span class="sxs-lookup"><span data-stu-id="23709-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="23709-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="23709-120">JSON Representation</span></span>
<span data-ttu-id="23709-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="23709-121">Here is a JSON representation of the resource.</span></span>
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
              "bundleID": "String"
            }
          ]
        }
      ]
    }
  ]
}
```




