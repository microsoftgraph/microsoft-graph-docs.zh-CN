---
title: managementCertificateWithThumbprint 资源类型
description: 尚未记录
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 765d3b9370e4b0f5eda481883956c72bf261e65a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418853"
---
# <a name="managementcertificatewiththumbprint-resource-type"></a><span data-ttu-id="a3a7d-103">managementCertificateWithThumbprint 资源类型</span><span class="sxs-lookup"><span data-stu-id="a3a7d-103">managementCertificateWithThumbprint resource type</span></span>

> <span data-ttu-id="a3a7d-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="a3a7d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a3a7d-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a3a7d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a3a7d-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a3a7d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a3a7d-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="a3a7d-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="a3a7d-108">属性</span><span class="sxs-lookup"><span data-stu-id="a3a7d-108">Properties</span></span>
|<span data-ttu-id="a3a7d-109">属性</span><span class="sxs-lookup"><span data-stu-id="a3a7d-109">Property</span></span>|<span data-ttu-id="a3a7d-110">类型</span><span class="sxs-lookup"><span data-stu-id="a3a7d-110">Type</span></span>|<span data-ttu-id="a3a7d-111">说明</span><span class="sxs-lookup"><span data-stu-id="a3a7d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a3a7d-112">指纹</span><span class="sxs-lookup"><span data-stu-id="a3a7d-112">thumbprint</span></span>|<span data-ttu-id="a3a7d-113">String</span><span class="sxs-lookup"><span data-stu-id="a3a7d-113">String</span></span>|<span data-ttu-id="a3a7d-114">管理证书的指纹</span><span class="sxs-lookup"><span data-stu-id="a3a7d-114">The thumbprint of the management certificate</span></span>|
|<span data-ttu-id="a3a7d-115">certificate</span><span class="sxs-lookup"><span data-stu-id="a3a7d-115">certificate</span></span>|<span data-ttu-id="a3a7d-116">String</span><span class="sxs-lookup"><span data-stu-id="a3a7d-116">String</span></span>|<span data-ttu-id="a3a7d-117">Base 64 编码的管理证书</span><span class="sxs-lookup"><span data-stu-id="a3a7d-117">The Base 64 encoded management certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="a3a7d-118">关系</span><span class="sxs-lookup"><span data-stu-id="a3a7d-118">Relationships</span></span>
<span data-ttu-id="a3a7d-119">无</span><span class="sxs-lookup"><span data-stu-id="a3a7d-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a3a7d-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a3a7d-120">JSON Representation</span></span>
<span data-ttu-id="a3a7d-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a3a7d-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managementCertificateWithThumbprint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managementCertificateWithThumbprint",
  "thumbprint": "String",
  "certificate": "String"
}
```




