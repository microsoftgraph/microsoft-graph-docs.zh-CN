---
title: extendedKeyUsage 资源类型
description: 自定义扩展密钥使用率定义
author: tfitzmac
ms.openlocfilehash: 2b6155a0fbb234cb0b2081a8a4a226a8d218dbc2
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27337287"
---
# <a name="extendedkeyusage-resource-type"></a><span data-ttu-id="21d52-103">extendedKeyUsage 资源类型</span><span class="sxs-lookup"><span data-stu-id="21d52-103">extendedKeyUsage resource type</span></span>

> <span data-ttu-id="21d52-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="21d52-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="21d52-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="21d52-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="21d52-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="21d52-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="21d52-107">自定义扩展密钥使用率定义</span><span class="sxs-lookup"><span data-stu-id="21d52-107">Custom Extended Key Usage definition</span></span>
## <a name="properties"></a><span data-ttu-id="21d52-108">属性</span><span class="sxs-lookup"><span data-stu-id="21d52-108">Properties</span></span>
|<span data-ttu-id="21d52-109">属性</span><span class="sxs-lookup"><span data-stu-id="21d52-109">Property</span></span>|<span data-ttu-id="21d52-110">类型</span><span class="sxs-lookup"><span data-stu-id="21d52-110">Type</span></span>|<span data-ttu-id="21d52-111">说明</span><span class="sxs-lookup"><span data-stu-id="21d52-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21d52-112">name</span><span class="sxs-lookup"><span data-stu-id="21d52-112">name</span></span>|<span data-ttu-id="21d52-113">字符串</span><span class="sxs-lookup"><span data-stu-id="21d52-113">String</span></span>|<span data-ttu-id="21d52-114">扩展的密钥用法名称</span><span class="sxs-lookup"><span data-stu-id="21d52-114">Extended Key Usage Name</span></span>|
|<span data-ttu-id="21d52-115">objectIdentifier</span><span class="sxs-lookup"><span data-stu-id="21d52-115">objectIdentifier</span></span>|<span data-ttu-id="21d52-116">字符串</span><span class="sxs-lookup"><span data-stu-id="21d52-116">String</span></span>|<span data-ttu-id="21d52-117">扩展密钥用法对象标识符</span><span class="sxs-lookup"><span data-stu-id="21d52-117">Extended Key Usage Object Identifier</span></span>|

## <a name="relationships"></a><span data-ttu-id="21d52-118">Relationships</span><span class="sxs-lookup"><span data-stu-id="21d52-118">Relationships</span></span>
<span data-ttu-id="21d52-119">无</span><span class="sxs-lookup"><span data-stu-id="21d52-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="21d52-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="21d52-120">JSON Representation</span></span>
<span data-ttu-id="21d52-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="21d52-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.extendedKeyUsage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.extendedKeyUsage",
  "name": "String",
  "objectIdentifier": "String"
}
```





