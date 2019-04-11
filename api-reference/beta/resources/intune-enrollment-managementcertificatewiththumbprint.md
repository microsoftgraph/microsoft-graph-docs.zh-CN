---
title: managementCertificateWithThumbprint 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 58b45f092848be7198141a34a443471426be273b
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31773705"
---
# <a name="managementcertificatewiththumbprint-resource-type"></a><span data-ttu-id="3e2d5-103">managementCertificateWithThumbprint 资源类型</span><span class="sxs-lookup"><span data-stu-id="3e2d5-103">managementCertificateWithThumbprint resource type</span></span>

> <span data-ttu-id="3e2d5-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3e2d5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3e2d5-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3e2d5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3e2d5-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="3e2d5-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="3e2d5-107">属性</span><span class="sxs-lookup"><span data-stu-id="3e2d5-107">Properties</span></span>
|<span data-ttu-id="3e2d5-108">属性</span><span class="sxs-lookup"><span data-stu-id="3e2d5-108">Property</span></span>|<span data-ttu-id="3e2d5-109">类型</span><span class="sxs-lookup"><span data-stu-id="3e2d5-109">Type</span></span>|<span data-ttu-id="3e2d5-110">说明</span><span class="sxs-lookup"><span data-stu-id="3e2d5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3e2d5-111">为</span><span class="sxs-lookup"><span data-stu-id="3e2d5-111">thumbprint</span></span>|<span data-ttu-id="3e2d5-112">String</span><span class="sxs-lookup"><span data-stu-id="3e2d5-112">String</span></span>|<span data-ttu-id="3e2d5-113">管理证书的指纹</span><span class="sxs-lookup"><span data-stu-id="3e2d5-113">The thumbprint of the management certificate</span></span>|
|<span data-ttu-id="3e2d5-114">证书</span><span class="sxs-lookup"><span data-stu-id="3e2d5-114">certificate</span></span>|<span data-ttu-id="3e2d5-115">String</span><span class="sxs-lookup"><span data-stu-id="3e2d5-115">String</span></span>|<span data-ttu-id="3e2d5-116">基本64编码管理证书</span><span class="sxs-lookup"><span data-stu-id="3e2d5-116">The Base 64 encoded management certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="3e2d5-117">关系</span><span class="sxs-lookup"><span data-stu-id="3e2d5-117">Relationships</span></span>
<span data-ttu-id="3e2d5-118">无</span><span class="sxs-lookup"><span data-stu-id="3e2d5-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3e2d5-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3e2d5-119">JSON Representation</span></span>
<span data-ttu-id="3e2d5-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3e2d5-120">Here is a JSON representation of the resource.</span></span>
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





