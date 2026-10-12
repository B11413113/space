# space

115-1 學期微算機原理及應用課程－程式碼與專案目錄。

---

## 專案檔案結構

<details>
<summary><a href="https://github.com/B11413113/space">space</a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;# 專案根目錄</summary>
<ul>
  <li>
    <details>
      <summary><a href="https://github.com/B11413113/space">.settings</a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;# Eclipse/STM32CubeIDE 專案編譯與除錯設定資料夾</summary>
      <ul>
        <li><a href="https://github.com/B11413113/space">language.settings.xml</a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;# C/C++ 語言編譯器語法解析配置</li>
      </ul>
    </details>
  </li>
  <li>
    <details>
      <summary><a href="https://github.com/B11413113/space">Core</a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;# 核心應用程式碼目錄</summary>
      <ul>
        <li>
          <details>
            <summary><a href="https://github.com/B11413113/space">Inc</a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;# 專案標頭檔目錄</summary>
            <ul>
              <li><a href="https://github.com/B11413113/space">main.h</a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;# 主程式全域標頭檔與 GPIO 引腳定義 (PA12, PB11, PB12 等)</li>
              <li><a href="https://github.com/B11413113/space">stm32g4xx_hal_conf.h</a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;# STM32 HAL 模組啟用與時脈參數配置檔</li>
              <li><a href="https://github.com/B11413113/space">stm32g4xx_it.h</a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;# 中斷服務常式函數原型宣告檔</li>
            </ul>
          </details>
        </li>
        <li>
          <details>
            <summary><a href="https://github.com/B11413113/space">Src</a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;# 專案 C 語言原始碼目錄</summary>
            <ul>
              <li><a href="https://github.com/B11413113/space">main.c</a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;# 主程式進入點、系統時脈初始化與按鍵輪詢狀態機邏輯</li>
              <li><a href="https://github.com/B11413113/space">stm32g4xx_hal_msp.c</a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;# MCU 底層外設 GPIO 初始化 (MSP) 實作</li>
              <li><a href="https://github.com/B11413113/space">stm32g4xx_it.c</a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;# Cortex-M4 系統異常與中斷服務常式實作</li>
              <li><a href="https://github.com/B11413113/space">system_stm32g4xx.c</a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;# STM32G4 系統時脈 (RCC/PLL) 設定與啟動邏輯</li>
            </ul>
          </details>
        </li>
        <li>
          <details>
            <summary><a href="https://github.com/B11413113/space">Startup</a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;# 開機啟動檔目錄</summary>
            <ul>
              <li><a href="https://github.com/B11413113/space">startup_stm32g474retx.s</a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;# ARM Assembly 組合語言啟動檔（設定 SP、向量表與進入 main）</li>
            </ul>
          </details>
        </li>
      </ul>
    </details>
  </li>
  <li>
    <details>
      <summary><a href="https://github.com/B11413113/space">Drivers</a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;# STM32 官方硬體驅動庫</summary>
      <ul>
        <li>
          <details>
            <summary><a href="https://github.com/B11413113/space">CMSIS</a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;# ARM Cortex-M 核心標準硬體抽象層</summary>
            <ul>
              <li><a href="https://github.com/B11413113/space">Device/ST/STM32G4xx/Include</a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;# STM32G4 暫存器結構與位址對映標頭檔</li>
              <li><a href="https://github.com/B11413113/space">Include</a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;# Cortex-M4 NVIC、SysTick 與 Core 內部暫存器標頭檔</li>
            </ul>
          </details>
        </li>
        <li>
          <details>
            <summary><a href="https://github.com/B11413113/space">STM32G4xx_HAL_Driver</a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;# ST 官方 HAL C 語言驅動程式庫</summary>
            <ul>
              <li><a href="https://github.com/B11413113/space">Inc</a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;# HAL 驅動庫標頭檔 (stm32g4xx_hal_gpio.h, rcc.h 等)</li>
              <li><a href="https://github.com/B11413113/space">Src</a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;# HAL 驅動庫原始碼 (stm32g4xx_hal_gpio.c, rcc.c 等)</li>
            </ul>
          </details>
        </li>
      </ul>
    </details>
  </li>
  <li>
    <details>
      <summary><a href="https://github.com/B11413113/space">Debug</a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;# 編譯產出與除錯檔目錄</summary>
      <ul>
        <li><a href="https://github.com/B11413113/space">Microcomputer_115_1.elf</a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;# 包含除錯資訊的可執行檔</li>
        <li><a href="https://github.com/B11413113/space">Microcomputer_115_1.hex</a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;# 可燒錄至 MCU Flash 的十六進制唯讀燒錄檔</li>
        <li><a href="https://github.com/B11413113/space">Microcomputer_115_1.map</a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;# 記憶體配置與位址映射表檔</li>
      </ul>
    </details>
  </li>
  <li><a href="https://github.com/B11413113/space">.cproject</a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;# STM32CubeIDE C/C++ 專案編譯路徑與工具鏈配置檔</li>
  <li><a href="https://github.com/B11413113/space">.project</a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;# Eclipse 專案識別與結構配置檔</li>
  <li><a href="https://github.com/B11413113/space">Microcomputer_115_1.ioc</a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;# STM32CubeMX 引腳對映、RCC 時脈與專案產生器設定檔</li>
  <li><a href="https://github.com/B11413113/space">STM32G474RETX_FLASH.ld</a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;# Linker 連結器腳本（定義 Flash 與 SRAM 位址分配）</li>
  <li><a href="https://github.com/B11413113/space/blob/main/Lab2.c">Lab2.c</a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;# 實驗二 C 語言程式碼檔案</li>
  <li><a href="https://github.com/B11413113/space/blob/main/lab3.txt">lab3.txt</a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;# 實驗三相關文字紀錄與說明檔案</li>
  <li><a href="https://github.com/B11413113/space/blob/main/work.txt">work.txt</a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;# 專案作業或開發筆記紀錄檔案</li>
  <li><a href="https://github.com/B11413113/space/blob/main/.gitattributes">.gitattributes</a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;# Git 檔案屬性設定檔</li>
  <li><a href="https://github.com/B11413113/space/blob/main/.gitignore">.gitignore</a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;# Git 忽略版本控制設定檔（包含暫存檔過濾）</li>
  <li><a href="https://github.com/B11413113/space/blob/main/README.md">README.md</a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;# 本儲存庫主說明文件</li>
</ul>
</details>