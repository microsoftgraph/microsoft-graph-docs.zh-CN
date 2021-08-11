---
title: deviceHealthAttestationState 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2a96ace9f81e9887dea36ef8ae6688bfbdc2ef96c4c8c97797c8e1417e426453
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54124351"
---
# <a name="devicehealthattestationstate-resource-type"></a>deviceHealthAttestationState 资源类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

尚未记录

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|lastUpdateDateTime|String|上次更新时间戳。|
|contentNamespaceUrl|String|DHA 报告版本。 （命名空间版本）|
|deviceHealthAttestationStatus|String|DHA 报告版本。 （命名空间版本）|
|contentVersion|String|HealthAttestation 状态架构版本|
|issuedDateTime|DateTimeOffset|评估设备或颁发给 MDM 的日期/时间|
|attestationIdentityKey|String|当设备上存在证明标识密钥 (AIK) 时，它表示设备具有认可密钥 (EK) 证书。|
|resetCount|Int64|电脑设备已休眠或恢复的次数|
|restartCount|Int64|电脑设备已重新启动的次数|
|dataExcutionPolicy|String|DEP 策略定义一组对内存执行额外检查的硬件和软件技术 |
|bitLockerStatus|String|BitLocker 驱动器加密开启或关闭|
|bootManagerVersion|String|引导管理器的版本|
|codeIntegrityCheckVersion|String|引导管理器的版本|
|secureBoot|String|启用安全启动后，核心组件必须具有正确的加密签名|
|bootDebugging|String|启用 bootDebugging 后，该设备用于开发和测试|
|operatingSystemKernelDebugging|String|启用 operatingSystemKernelDebugging 后，该设备用于开发和测试|
|codeIntegrity|String| 启用代码完整性后，代码执行限于完整性已验证的代码|
|testSigning|String|当允许测试签名时，设备不会在引导期间强制执行签名验证|
|safeMode|String|安全模式是 Windows 的一种故障排除选项，用于在受限状态下启动计算机|
|windowsPE|String|运行受限服务的操作系统，用于为 Windows 准备计算机|
|earlyLaunchAntiMalwareDriverProtection|String|ELAM 为网络中的计算机启动时提供保护|
|virtualSecureMode|String|VSM 是一个容器，可以保护高价值资产免受已损坏内核的威胁|
|pcrHashAlgorithm|String|标识 TPM 使用的 HASH 算法的信息属性|
|bootAppSecurityVersion|String|启动应用程序的安全版本号|
|bootManagerSecurityVersion|String|启动应用程序的安全版本号|
|tpmVersion|String|启动应用程序的安全版本号|
|pcr0|String|在 PCR\[0\] 中捕获的度量|
|secureBootConfigurationPolicyFingerPrint|String|自定义安全启动配置策略的指纹|
|codeIntegrityPolicy|String|控制启动环境安全性的代码完整性策略|
|bootRevisionListInfo|String|在已证明的设备上进行初始启动期间加载的启动修订列表|
|operatingSystemRevListInfo|String|在已证明的设备上进行初始启动期间加载的操作系统修订列表|
|healthStatusMismatchInfo|String|如果 DHA 服务检测到完整性问题，则此属性会出现|
|healthAttestationSupportedStatus|String|此属性指示设备是否支持 DHA|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceHealthAttestationState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthAttestationState",
  "lastUpdateDateTime": "String",
  "contentNamespaceUrl": "String",
  "deviceHealthAttestationStatus": "String",
  "contentVersion": "String",
  "issuedDateTime": "String (timestamp)",
  "attestationIdentityKey": "String",
  "resetCount": 1024,
  "restartCount": 1024,
  "dataExcutionPolicy": "String",
  "bitLockerStatus": "String",
  "bootManagerVersion": "String",
  "codeIntegrityCheckVersion": "String",
  "secureBoot": "String",
  "bootDebugging": "String",
  "operatingSystemKernelDebugging": "String",
  "codeIntegrity": "String",
  "testSigning": "String",
  "safeMode": "String",
  "windowsPE": "String",
  "earlyLaunchAntiMalwareDriverProtection": "String",
  "virtualSecureMode": "String",
  "pcrHashAlgorithm": "String",
  "bootAppSecurityVersion": "String",
  "bootManagerSecurityVersion": "String",
  "tpmVersion": "String",
  "pcr0": "String",
  "secureBootConfigurationPolicyFingerPrint": "String",
  "codeIntegrityPolicy": "String",
  "bootRevisionListInfo": "String",
  "operatingSystemRevListInfo": "String",
  "healthStatusMismatchInfo": "String",
  "healthAttestationSupportedStatus": "String"
}
```




