---
title: managementCertificateWithThumbprint 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: fa78c594179edcd5a1cf4bc1b6e331d95155fc4e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48079919"
---
# <a name="managementcertificatewiththumbprint-resource-type"></a><span data-ttu-id="8ff97-103">managementCertificateWithThumbprint 资源类型</span><span class="sxs-lookup"><span data-stu-id="8ff97-103">managementCertificateWithThumbprint resource type</span></span>

<span data-ttu-id="8ff97-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8ff97-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8ff97-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8ff97-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8ff97-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8ff97-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8ff97-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="8ff97-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="8ff97-108">属性</span><span class="sxs-lookup"><span data-stu-id="8ff97-108">Properties</span></span>
|<span data-ttu-id="8ff97-109">属性</span><span class="sxs-lookup"><span data-stu-id="8ff97-109">Property</span></span>|<span data-ttu-id="8ff97-110">类型</span><span class="sxs-lookup"><span data-stu-id="8ff97-110">Type</span></span>|<span data-ttu-id="8ff97-111">说明</span><span class="sxs-lookup"><span data-stu-id="8ff97-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8ff97-112">为</span><span class="sxs-lookup"><span data-stu-id="8ff97-112">thumbprint</span></span>|<span data-ttu-id="8ff97-113">String</span><span class="sxs-lookup"><span data-stu-id="8ff97-113">String</span></span>|<span data-ttu-id="8ff97-114">管理证书的指纹</span><span class="sxs-lookup"><span data-stu-id="8ff97-114">The thumbprint of the management certificate</span></span>|
|<span data-ttu-id="8ff97-115">证书</span><span class="sxs-lookup"><span data-stu-id="8ff97-115">certificate</span></span>|<span data-ttu-id="8ff97-116">String</span><span class="sxs-lookup"><span data-stu-id="8ff97-116">String</span></span>|<span data-ttu-id="8ff97-117">基本64编码管理证书</span><span class="sxs-lookup"><span data-stu-id="8ff97-117">The Base 64 encoded management certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="8ff97-118">关系</span><span class="sxs-lookup"><span data-stu-id="8ff97-118">Relationships</span></span>
<span data-ttu-id="8ff97-119">无</span><span class="sxs-lookup"><span data-stu-id="8ff97-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8ff97-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8ff97-120">JSON Representation</span></span>
<span data-ttu-id="8ff97-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8ff97-121">Here is a JSON representation of the resource.</span></span>
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






