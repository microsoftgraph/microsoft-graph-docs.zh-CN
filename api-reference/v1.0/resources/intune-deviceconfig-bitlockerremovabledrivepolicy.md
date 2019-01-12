---
title: bitLockerRemovableDrivePolicy 资源类型
description: BitLocker 可移动驱动器策略。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 040f4230cf1d3aab02f97237b88093126f8dc24c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27926335"
---
# <a name="bitlockerremovabledrivepolicy-resource-type"></a><span data-ttu-id="9c685-103">bitLockerRemovableDrivePolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="9c685-103">bitLockerRemovableDrivePolicy resource type</span></span>

> <span data-ttu-id="9c685-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="9c685-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9c685-105">BitLocker 可移动驱动器策略。</span><span class="sxs-lookup"><span data-stu-id="9c685-105">BitLocker Removable Drive Policies.</span></span>
## <a name="properties"></a><span data-ttu-id="9c685-106">属性</span><span class="sxs-lookup"><span data-stu-id="9c685-106">Properties</span></span>
|<span data-ttu-id="9c685-107">属性</span><span class="sxs-lookup"><span data-stu-id="9c685-107">Property</span></span>|<span data-ttu-id="9c685-108">类型</span><span class="sxs-lookup"><span data-stu-id="9c685-108">Type</span></span>|<span data-ttu-id="9c685-109">说明</span><span class="sxs-lookup"><span data-stu-id="9c685-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9c685-110">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="9c685-110">encryptionMethod</span></span>|[<span data-ttu-id="9c685-111">bitLockerEncryptionMethod</span><span class="sxs-lookup"><span data-stu-id="9c685-111">bitLockerEncryptionMethod</span></span>](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|<span data-ttu-id="9c685-112">选择可移动驱动器的加密方法。</span><span class="sxs-lookup"><span data-stu-id="9c685-112">Select the encryption method for removable  drives.</span></span> <span data-ttu-id="9c685-113">可取值为：`aesCbc128`、`aesCbc256`、`xtsAes128`、`xtsAes256`</span><span class="sxs-lookup"><span data-stu-id="9c685-113">Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span></span>|
|<span data-ttu-id="9c685-114">requireEncryptionForWriteAccess</span><span class="sxs-lookup"><span data-stu-id="9c685-114">requireEncryptionForWriteAccess</span></span>|<span data-ttu-id="9c685-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="9c685-115">Boolean</span></span>|<span data-ttu-id="9c685-116">指示是否阻止对其他组织中配置的设备的写入权限。</span><span class="sxs-lookup"><span data-stu-id="9c685-116">Indicates whether to block write access to devices configured in another organization.</span></span>  <span data-ttu-id="9c685-117">如果 requireEncryptionForWriteAccess 为 false，则此值没有影响。</span><span class="sxs-lookup"><span data-stu-id="9c685-117">If requireEncryptionForWriteAccess is false, this value does not affect.</span></span>|
|<span data-ttu-id="9c685-118">blockCrossOrganizationWriteAccess</span><span class="sxs-lookup"><span data-stu-id="9c685-118">blockCrossOrganizationWriteAccess</span></span>|<span data-ttu-id="9c685-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="9c685-119">Boolean</span></span>|<span data-ttu-id="9c685-120">此策略设置决定可移动数据驱动器是否需要 BitLocker 保护，以使其在计算机上可写。</span><span class="sxs-lookup"><span data-stu-id="9c685-120">This policy setting determines whether BitLocker protection is required for removable data drives to be writable on a computer.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9c685-121">关系</span><span class="sxs-lookup"><span data-stu-id="9c685-121">Relationships</span></span>
<span data-ttu-id="9c685-122">无</span><span class="sxs-lookup"><span data-stu-id="9c685-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9c685-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9c685-123">JSON Representation</span></span>
<span data-ttu-id="9c685-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9c685-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.bitLockerRemovableDrivePolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bitLockerRemovableDrivePolicy",
  "encryptionMethod": "String",
  "requireEncryptionForWriteAccess": true,
  "blockCrossOrganizationWriteAccess": true
}
```



