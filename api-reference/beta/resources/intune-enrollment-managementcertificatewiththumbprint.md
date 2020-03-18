---
title: managementCertificateWithThumbprint 资源类型
description: 尚未记录
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e9fad4b5e129b81d4fba37c19f25d20b59e16236
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42783415"
---
# <a name="managementcertificatewiththumbprint-resource-type"></a><span data-ttu-id="9c26f-103">managementCertificateWithThumbprint 资源类型</span><span class="sxs-lookup"><span data-stu-id="9c26f-103">managementCertificateWithThumbprint resource type</span></span>

> <span data-ttu-id="9c26f-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9c26f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9c26f-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9c26f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9c26f-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="9c26f-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="9c26f-107">属性</span><span class="sxs-lookup"><span data-stu-id="9c26f-107">Properties</span></span>
|<span data-ttu-id="9c26f-108">属性</span><span class="sxs-lookup"><span data-stu-id="9c26f-108">Property</span></span>|<span data-ttu-id="9c26f-109">类型</span><span class="sxs-lookup"><span data-stu-id="9c26f-109">Type</span></span>|<span data-ttu-id="9c26f-110">说明</span><span class="sxs-lookup"><span data-stu-id="9c26f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9c26f-111">为</span><span class="sxs-lookup"><span data-stu-id="9c26f-111">thumbprint</span></span>|<span data-ttu-id="9c26f-112">String</span><span class="sxs-lookup"><span data-stu-id="9c26f-112">String</span></span>|<span data-ttu-id="9c26f-113">管理证书的指纹</span><span class="sxs-lookup"><span data-stu-id="9c26f-113">The thumbprint of the management certificate</span></span>|
|<span data-ttu-id="9c26f-114">证书</span><span class="sxs-lookup"><span data-stu-id="9c26f-114">certificate</span></span>|<span data-ttu-id="9c26f-115">String</span><span class="sxs-lookup"><span data-stu-id="9c26f-115">String</span></span>|<span data-ttu-id="9c26f-116">基本64编码管理证书</span><span class="sxs-lookup"><span data-stu-id="9c26f-116">The Base 64 encoded management certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="9c26f-117">关系</span><span class="sxs-lookup"><span data-stu-id="9c26f-117">Relationships</span></span>
<span data-ttu-id="9c26f-118">无</span><span class="sxs-lookup"><span data-stu-id="9c26f-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9c26f-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9c26f-119">JSON Representation</span></span>
<span data-ttu-id="9c26f-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9c26f-120">Here is a JSON representation of the resource.</span></span>
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



