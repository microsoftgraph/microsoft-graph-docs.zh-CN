---
title: managementCertificateWithThumbprint 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 6e6259c1f90547ff875fa31d3f383606749bc0dd
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27983350"
---
# <a name="managementcertificatewiththumbprint-resource-type"></a><span data-ttu-id="d9c00-103">managementCertificateWithThumbprint 资源类型</span><span class="sxs-lookup"><span data-stu-id="d9c00-103">managementCertificateWithThumbprint resource type</span></span>

> <span data-ttu-id="d9c00-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d9c00-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d9c00-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d9c00-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d9c00-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="d9c00-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d9c00-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d9c00-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="d9c00-108">属性</span><span class="sxs-lookup"><span data-stu-id="d9c00-108">Properties</span></span>
|<span data-ttu-id="d9c00-109">属性</span><span class="sxs-lookup"><span data-stu-id="d9c00-109">Property</span></span>|<span data-ttu-id="d9c00-110">类型</span><span class="sxs-lookup"><span data-stu-id="d9c00-110">Type</span></span>|<span data-ttu-id="d9c00-111">说明</span><span class="sxs-lookup"><span data-stu-id="d9c00-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d9c00-112">指纹</span><span class="sxs-lookup"><span data-stu-id="d9c00-112">thumbprint</span></span>|<span data-ttu-id="d9c00-113">字符串</span><span class="sxs-lookup"><span data-stu-id="d9c00-113">String</span></span>|<span data-ttu-id="d9c00-114">管理证书的指纹</span><span class="sxs-lookup"><span data-stu-id="d9c00-114">The thumbprint of the management certificate</span></span>|
|<span data-ttu-id="d9c00-115">certificate</span><span class="sxs-lookup"><span data-stu-id="d9c00-115">certificate</span></span>|<span data-ttu-id="d9c00-116">String</span><span class="sxs-lookup"><span data-stu-id="d9c00-116">String</span></span>|<span data-ttu-id="d9c00-117">Base 64 编码的管理证书</span><span class="sxs-lookup"><span data-stu-id="d9c00-117">The Base 64 encoded management certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="d9c00-118">Relationships</span><span class="sxs-lookup"><span data-stu-id="d9c00-118">Relationships</span></span>
<span data-ttu-id="d9c00-119">无</span><span class="sxs-lookup"><span data-stu-id="d9c00-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d9c00-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d9c00-120">JSON Representation</span></span>
<span data-ttu-id="d9c00-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d9c00-121">Here is a JSON representation of the resource.</span></span>
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





