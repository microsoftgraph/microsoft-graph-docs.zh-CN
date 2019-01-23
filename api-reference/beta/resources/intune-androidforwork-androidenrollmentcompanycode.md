---
title: androidEnrollmentCompanyCode 资源类型
description: 用于容纳专业注册数据用于注册通过 Google Android 管理 API，如令牌、 Url 和 QR 代码内容的类
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: be5b2a94445e95fe18271467b6661320d8204d76
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429313"
---
# <a name="androidenrollmentcompanycode-resource-type"></a><span data-ttu-id="f0712-103">androidEnrollmentCompanyCode 资源类型</span><span class="sxs-lookup"><span data-stu-id="f0712-103">androidEnrollmentCompanyCode resource type</span></span>

> <span data-ttu-id="f0712-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="f0712-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f0712-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f0712-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f0712-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f0712-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f0712-107">用于容纳专业注册数据用于注册通过 Google Android 管理 API，如令牌、 Url 和 QR 代码内容的类</span><span class="sxs-lookup"><span data-stu-id="f0712-107">A class to hold specialty enrollment data used for enrolling via Google's Android Management API, such as Token, Url, and QR code content</span></span>

## <a name="properties"></a><span data-ttu-id="f0712-108">属性</span><span class="sxs-lookup"><span data-stu-id="f0712-108">Properties</span></span>
|<span data-ttu-id="f0712-109">属性</span><span class="sxs-lookup"><span data-stu-id="f0712-109">Property</span></span>|<span data-ttu-id="f0712-110">类型</span><span class="sxs-lookup"><span data-stu-id="f0712-110">Type</span></span>|<span data-ttu-id="f0712-111">说明</span><span class="sxs-lookup"><span data-stu-id="f0712-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0712-112">enrollmentToken</span><span class="sxs-lookup"><span data-stu-id="f0712-112">enrollmentToken</span></span>|<span data-ttu-id="f0712-113">String</span><span class="sxs-lookup"><span data-stu-id="f0712-113">String</span></span>|<span data-ttu-id="f0712-114">注册用户用于注册其设备令牌。</span><span class="sxs-lookup"><span data-stu-id="f0712-114">Enrollment Token used by the User to enroll their device.</span></span>|
|<span data-ttu-id="f0712-115">qrCodeContent</span><span class="sxs-lookup"><span data-stu-id="f0712-115">qrCodeContent</span></span>|<span data-ttu-id="f0712-116">String</span><span class="sxs-lookup"><span data-stu-id="f0712-116">String</span></span>|<span data-ttu-id="f0712-117">用于生成此令牌的 QR 码的字符串。</span><span class="sxs-lookup"><span data-stu-id="f0712-117">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="f0712-118">qrCodeImage</span><span class="sxs-lookup"><span data-stu-id="f0712-118">qrCodeImage</span></span>|[<span data-ttu-id="f0712-119">mimeContent</span><span class="sxs-lookup"><span data-stu-id="f0712-119">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="f0712-120">生成的令牌 QR 代码。</span><span class="sxs-lookup"><span data-stu-id="f0712-120">Generated QR code for the token.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f0712-121">关系</span><span class="sxs-lookup"><span data-stu-id="f0712-121">Relationships</span></span>
<span data-ttu-id="f0712-122">无</span><span class="sxs-lookup"><span data-stu-id="f0712-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f0712-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f0712-123">JSON Representation</span></span>
<span data-ttu-id="f0712-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f0712-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidEnrollmentCompanyCode"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidEnrollmentCompanyCode",
  "enrollmentToken": "String",
  "qrCodeContent": "String",
  "qrCodeImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  }
}
```




