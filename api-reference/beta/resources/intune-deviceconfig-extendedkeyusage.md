---
title: extendedKeyUsage 资源类型
description: 自定义扩展密钥使用率定义
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6ed825f44923d3fe86cc410397747b50a1f2c681
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425965"
---
# <a name="extendedkeyusage-resource-type"></a><span data-ttu-id="f4694-103">extendedKeyUsage 资源类型</span><span class="sxs-lookup"><span data-stu-id="f4694-103">extendedKeyUsage resource type</span></span>

> <span data-ttu-id="f4694-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="f4694-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f4694-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f4694-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f4694-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f4694-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f4694-107">自定义扩展密钥使用率定义</span><span class="sxs-lookup"><span data-stu-id="f4694-107">Custom Extended Key Usage definition</span></span>

## <a name="properties"></a><span data-ttu-id="f4694-108">属性</span><span class="sxs-lookup"><span data-stu-id="f4694-108">Properties</span></span>
|<span data-ttu-id="f4694-109">属性</span><span class="sxs-lookup"><span data-stu-id="f4694-109">Property</span></span>|<span data-ttu-id="f4694-110">类型</span><span class="sxs-lookup"><span data-stu-id="f4694-110">Type</span></span>|<span data-ttu-id="f4694-111">说明</span><span class="sxs-lookup"><span data-stu-id="f4694-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4694-112">name</span><span class="sxs-lookup"><span data-stu-id="f4694-112">name</span></span>|<span data-ttu-id="f4694-113">String</span><span class="sxs-lookup"><span data-stu-id="f4694-113">String</span></span>|<span data-ttu-id="f4694-114">扩展的密钥用法名称</span><span class="sxs-lookup"><span data-stu-id="f4694-114">Extended Key Usage Name</span></span>|
|<span data-ttu-id="f4694-115">objectIdentifier</span><span class="sxs-lookup"><span data-stu-id="f4694-115">objectIdentifier</span></span>|<span data-ttu-id="f4694-116">String</span><span class="sxs-lookup"><span data-stu-id="f4694-116">String</span></span>|<span data-ttu-id="f4694-117">扩展密钥用法对象标识符</span><span class="sxs-lookup"><span data-stu-id="f4694-117">Extended Key Usage Object Identifier</span></span>|

## <a name="relationships"></a><span data-ttu-id="f4694-118">关系</span><span class="sxs-lookup"><span data-stu-id="f4694-118">Relationships</span></span>
<span data-ttu-id="f4694-119">无</span><span class="sxs-lookup"><span data-stu-id="f4694-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f4694-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f4694-120">JSON Representation</span></span>
<span data-ttu-id="f4694-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f4694-121">Here is a JSON representation of the resource.</span></span>
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




